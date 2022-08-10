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
$ docker pull caddy@sha256:04275786ace772b2bd49b3be4c692739aa6e3912b7cee35ac3e25dae660fba4a
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
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:bf37b595db36a904158da15138010561a6e121052e21f56aacbcc3cdf36e50c2
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
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:bb4ffc190f522d40ab390008e988db6e281e629e2363deb7e741a012d46d6488
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
$ docker pull caddy@sha256:4f6505a47382b5dec53662e2690f8f2c92c421c3183d6eadc0a2813923a33654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126629543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce17ec8cd808074c0b242c463275fec3b0882f6e530f6697c7c144b944d365d`
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
# Tue, 09 Aug 2022 19:15:05 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:16:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:16:41 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:16:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:16:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:16:42 GMT
WORKDIR /go
# Wed, 10 Aug 2022 02:26:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 02:26:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 02:26:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 02:26:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 02:26:07 GMT
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
	-	`sha256:af72e8bb74dba7b7a51456e414ac4999ff55a6a68e532a7cd1b6f32707be625f`  
		Last Modified: Tue, 09 Aug 2022 19:21:02 GMT  
		Size: 115.3 MB (115307225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421caacf35538ce671745cb9396eea38bf42cd3093eaf78dbcbe8bf5f83f82`  
		Last Modified: Tue, 09 Aug 2022 19:20:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06697ac7525490322e188b4b7c69500be186a38b1e83fc958cc4867577c89158`  
		Last Modified: Wed, 10 Aug 2022 02:26:41 GMT  
		Size: 6.9 MB (6941419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5272157df3949dde928ea90eaa0635d68c0e26b948696969f0ba100479f29d`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 1.3 MB (1289405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b2b76ccc7cb5ba98c8767f67ac01f45277649a0811109b81e23a55f84b2a5c`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e0bf3bb2f59bf72edcc69c72a3f95c05cae17d0dec32c3d2cdab3fd6fb45f6d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122605921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b23231332ede1e79114d2bcb35b96798016a2d8f1a3a5982908b631f73fc78a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 16:49:24 GMT
RUN apk add --no-cache ca-certificates
# Mon, 01 Aug 2022 16:49:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 16:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:04:45 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:13:52 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:13:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:13:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:13:53 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:53:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:53:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:53:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:53:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6060c9d5374931abb20ecd8e9328461917403d9561724f3df09c7e3fc87e8d7d`  
		Last Modified: Mon, 01 Aug 2022 17:33:54 GMT  
		Size: 284.7 KB (284743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc4259925cc07fecc6dc2421bf221853fe7ba33c4e1e630be41c927f23d5c05`  
		Last Modified: Mon, 01 Aug 2022 17:33:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42697db054e71ef6e42dc53a7b6145ae161eec6b80ac859c94ea018d09946540`  
		Last Modified: Mon, 01 Aug 2022 17:35:37 GMT  
		Size: 111.7 MB (111676715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc53c3f06fa91cdb79713efceaac7e9827d7848ed8c57d7fda971c1600072b6`  
		Last Modified: Mon, 01 Aug 2022 17:35:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020874bca98f79f6a60a6924e96c8fdf2ca45b4b3c0db0dea618c8e3d8c18ba`  
		Last Modified: Mon, 01 Aug 2022 17:54:26 GMT  
		Size: 6.8 MB (6808158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603ca030f2449d834b67ff449623a1cc9bb19d714d73c871eb89d39128826cfa`  
		Last Modified: Mon, 01 Aug 2022 17:54:25 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1699d137e1da0fc21e7af9c97fb58dd7c2e308a696d3669504d8ea4a2f9e62`  
		Last Modified: Mon, 01 Aug 2022 17:54:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bfa292826e8a20c33c3bf5175a0a10856b37d2fdf8a5ea891afbb9f863a1f13a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121428778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a30fdc400c6c38966a73f29da6af28b7751f8b2198b179292c2337837bdb884`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:59:34 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:08:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:08:40 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:08:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:54:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:54:18 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:54:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:54:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:54:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21b88218f56922c09b90952709a63bdecdde1ad2b4862aa7a697bbc578fecc`  
		Last Modified: Mon, 01 Aug 2022 17:35:21 GMT  
		Size: 111.4 MB (111449451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80adfea5b864e9bad4d701d93f87eedc3d89d7f508bdca67c613fdd65f46a1`  
		Last Modified: Mon, 01 Aug 2022 17:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134dbd094d15baa4d9e81748348ff6846c5d408a0fa5c195ae63f1e358ccdb`  
		Last Modified: Mon, 01 Aug 2022 17:54:58 GMT  
		Size: 6.1 MB (6067302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a36468cc7f395bc290ce04c2216468804fa13342fe0a49779a055958e9cb4c4`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 1.2 MB (1228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b67e6165d74b155d0ffc5f7a4cc9990cba565802b8ed0c9d754c3fb1ccffa2`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd8f1bce5198290bc50b08a93155ac38199a9dae48210ccfd5a4a41f5a95e19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121553906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ba051875de5f211ec4507df16e581228bf4219831d0589611b865a52455e5`
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
# Tue, 09 Aug 2022 19:11:57 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:13:28 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:13:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:13:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:13:31 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:52:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:52:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:52:15 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:52:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:52:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:52:20 GMT
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
	-	`sha256:cea4debaad2864fd0099780f6208841dc3a80054b81f7531944737f0f633e22a`  
		Last Modified: Tue, 09 Aug 2022 19:18:08 GMT  
		Size: 110.3 MB (110319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316bf57efd3b0cdd0835f8d3393e898cd27ed09707eff97189df62f132805299`  
		Last Modified: Tue, 09 Aug 2022 19:17:51 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a06f48c9f0345985d2098cac6d089f1580a8d87b4a2a782eb7bfbee426aef`  
		Last Modified: Wed, 10 Aug 2022 06:52:52 GMT  
		Size: 7.1 MB (7052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8265fec039b8677f92210d7029a762398511c9280be7d4d0efc1cb10be17d`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 1.2 MB (1189008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb8a803f3f8d02849a88c0ce723f1c41d644bba7cb86e8a8cf77a0ad559083e`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f17a6fc6ee71b48c6ad47db82361ca9e27fa68f51051efe89a989043228eca84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122067226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5d604a3361c5c0060249fcfc23e6dfa6eac3e105171f0a9c69e1f00e634c1`
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
# Tue, 09 Aug 2022 18:21:28 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:24:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:24:15 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:24:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:24:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:24:16 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:18:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:18:49 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:18:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:18:52 GMT
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
	-	`sha256:cf877b37b50b5ec020497c8c6cacab5479917d459e740c6380a0a14425d6ab8f`  
		Last Modified: Tue, 09 Aug 2022 18:30:52 GMT  
		Size: 110.3 MB (110317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15924e03aa834b25daf0b7536184d4b2e54a7463f9410eaca0d81764df5c962`  
		Last Modified: Tue, 09 Aug 2022 18:30:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70115b37e266a1fa2567feb847cdccaa6a8b04ef98c4fbe797713b9801bb31be`  
		Last Modified: Wed, 10 Aug 2022 06:19:29 GMT  
		Size: 7.5 MB (7482240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae18e224805e17c6354f387924797ff18689005d909dd3a998ca3ed86195a9d`  
		Last Modified: Wed, 10 Aug 2022 06:19:28 GMT  
		Size: 1.2 MB (1176360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458775e44b7b881bad4eb74564e5d89bf1a652b0a6139b393470e3947511522`  
		Last Modified: Wed, 10 Aug 2022 06:19:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ef260a1ad1352465c56c4f64504134432b8d3d143338c3e3f1d28b4baa38c6c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124362245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cdcf841b6257118f75389e3e0e2aa3be06c392d0847687846d270d30cfeeab`
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
# Tue, 09 Aug 2022 18:49:40 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:51:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:51:26 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:51:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:51:27 GMT
WORKDIR /go
# Wed, 10 Aug 2022 08:14:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 08:14:21 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 08:14:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 08:14:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 08:14:22 GMT
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
	-	`sha256:370520e38e9ed965c5d2cd2daaf4431f1d2a9806663edc24c91e7137673ddcbc`  
		Last Modified: Tue, 09 Aug 2022 18:56:17 GMT  
		Size: 113.2 MB (113190080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcdedfdcc75de69b3488999d0229cde87827f3a07d2a8f28e869413f71bd5c4`  
		Last Modified: Tue, 09 Aug 2022 18:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848bc4e4bc8147cbd275c615d51ec5163fbc2b82705ed1bba9ef58237b93bf1d`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 7.1 MB (7052782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5214650dd00d68f62fb6dd06529a360c4a2c6c24185c341b9f880d91ef775438`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e086fc28f8c601de8cdf5365d27a0ae8546d116fcf03e99d3b823bac7f9047`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 405.0 B  
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

### `caddy:2-builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
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
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
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
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:909a8efd2efb13ed2cd838b6c396e22e10b70018d9a4d332c28fa1079402e9c5
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
$ docker pull caddy@sha256:4f6505a47382b5dec53662e2690f8f2c92c421c3183d6eadc0a2813923a33654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126629543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce17ec8cd808074c0b242c463275fec3b0882f6e530f6697c7c144b944d365d`
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
# Tue, 09 Aug 2022 19:15:05 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:16:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:16:41 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:16:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:16:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:16:42 GMT
WORKDIR /go
# Wed, 10 Aug 2022 02:26:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 02:26:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 02:26:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 02:26:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 02:26:07 GMT
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
	-	`sha256:af72e8bb74dba7b7a51456e414ac4999ff55a6a68e532a7cd1b6f32707be625f`  
		Last Modified: Tue, 09 Aug 2022 19:21:02 GMT  
		Size: 115.3 MB (115307225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421caacf35538ce671745cb9396eea38bf42cd3093eaf78dbcbe8bf5f83f82`  
		Last Modified: Tue, 09 Aug 2022 19:20:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06697ac7525490322e188b4b7c69500be186a38b1e83fc958cc4867577c89158`  
		Last Modified: Wed, 10 Aug 2022 02:26:41 GMT  
		Size: 6.9 MB (6941419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5272157df3949dde928ea90eaa0635d68c0e26b948696969f0ba100479f29d`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 1.3 MB (1289405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b2b76ccc7cb5ba98c8767f67ac01f45277649a0811109b81e23a55f84b2a5c`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e0bf3bb2f59bf72edcc69c72a3f95c05cae17d0dec32c3d2cdab3fd6fb45f6d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122605921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b23231332ede1e79114d2bcb35b96798016a2d8f1a3a5982908b631f73fc78a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 16:49:24 GMT
RUN apk add --no-cache ca-certificates
# Mon, 01 Aug 2022 16:49:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 16:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:04:45 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:13:52 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:13:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:13:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:13:53 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:53:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:53:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:53:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:53:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6060c9d5374931abb20ecd8e9328461917403d9561724f3df09c7e3fc87e8d7d`  
		Last Modified: Mon, 01 Aug 2022 17:33:54 GMT  
		Size: 284.7 KB (284743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc4259925cc07fecc6dc2421bf221853fe7ba33c4e1e630be41c927f23d5c05`  
		Last Modified: Mon, 01 Aug 2022 17:33:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42697db054e71ef6e42dc53a7b6145ae161eec6b80ac859c94ea018d09946540`  
		Last Modified: Mon, 01 Aug 2022 17:35:37 GMT  
		Size: 111.7 MB (111676715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc53c3f06fa91cdb79713efceaac7e9827d7848ed8c57d7fda971c1600072b6`  
		Last Modified: Mon, 01 Aug 2022 17:35:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020874bca98f79f6a60a6924e96c8fdf2ca45b4b3c0db0dea618c8e3d8c18ba`  
		Last Modified: Mon, 01 Aug 2022 17:54:26 GMT  
		Size: 6.8 MB (6808158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603ca030f2449d834b67ff449623a1cc9bb19d714d73c871eb89d39128826cfa`  
		Last Modified: Mon, 01 Aug 2022 17:54:25 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1699d137e1da0fc21e7af9c97fb58dd7c2e308a696d3669504d8ea4a2f9e62`  
		Last Modified: Mon, 01 Aug 2022 17:54:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bfa292826e8a20c33c3bf5175a0a10856b37d2fdf8a5ea891afbb9f863a1f13a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121428778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a30fdc400c6c38966a73f29da6af28b7751f8b2198b179292c2337837bdb884`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:59:34 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:08:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:08:40 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:08:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:54:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:54:18 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:54:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:54:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:54:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21b88218f56922c09b90952709a63bdecdde1ad2b4862aa7a697bbc578fecc`  
		Last Modified: Mon, 01 Aug 2022 17:35:21 GMT  
		Size: 111.4 MB (111449451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80adfea5b864e9bad4d701d93f87eedc3d89d7f508bdca67c613fdd65f46a1`  
		Last Modified: Mon, 01 Aug 2022 17:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134dbd094d15baa4d9e81748348ff6846c5d408a0fa5c195ae63f1e358ccdb`  
		Last Modified: Mon, 01 Aug 2022 17:54:58 GMT  
		Size: 6.1 MB (6067302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a36468cc7f395bc290ce04c2216468804fa13342fe0a49779a055958e9cb4c4`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 1.2 MB (1228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b67e6165d74b155d0ffc5f7a4cc9990cba565802b8ed0c9d754c3fb1ccffa2`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd8f1bce5198290bc50b08a93155ac38199a9dae48210ccfd5a4a41f5a95e19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121553906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ba051875de5f211ec4507df16e581228bf4219831d0589611b865a52455e5`
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
# Tue, 09 Aug 2022 19:11:57 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:13:28 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:13:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:13:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:13:31 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:52:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:52:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:52:15 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:52:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:52:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:52:20 GMT
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
	-	`sha256:cea4debaad2864fd0099780f6208841dc3a80054b81f7531944737f0f633e22a`  
		Last Modified: Tue, 09 Aug 2022 19:18:08 GMT  
		Size: 110.3 MB (110319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316bf57efd3b0cdd0835f8d3393e898cd27ed09707eff97189df62f132805299`  
		Last Modified: Tue, 09 Aug 2022 19:17:51 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a06f48c9f0345985d2098cac6d089f1580a8d87b4a2a782eb7bfbee426aef`  
		Last Modified: Wed, 10 Aug 2022 06:52:52 GMT  
		Size: 7.1 MB (7052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8265fec039b8677f92210d7029a762398511c9280be7d4d0efc1cb10be17d`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 1.2 MB (1189008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb8a803f3f8d02849a88c0ce723f1c41d644bba7cb86e8a8cf77a0ad559083e`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f17a6fc6ee71b48c6ad47db82361ca9e27fa68f51051efe89a989043228eca84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122067226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5d604a3361c5c0060249fcfc23e6dfa6eac3e105171f0a9c69e1f00e634c1`
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
# Tue, 09 Aug 2022 18:21:28 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:24:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:24:15 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:24:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:24:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:24:16 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:18:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:18:49 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:18:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:18:52 GMT
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
	-	`sha256:cf877b37b50b5ec020497c8c6cacab5479917d459e740c6380a0a14425d6ab8f`  
		Last Modified: Tue, 09 Aug 2022 18:30:52 GMT  
		Size: 110.3 MB (110317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15924e03aa834b25daf0b7536184d4b2e54a7463f9410eaca0d81764df5c962`  
		Last Modified: Tue, 09 Aug 2022 18:30:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70115b37e266a1fa2567feb847cdccaa6a8b04ef98c4fbe797713b9801bb31be`  
		Last Modified: Wed, 10 Aug 2022 06:19:29 GMT  
		Size: 7.5 MB (7482240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae18e224805e17c6354f387924797ff18689005d909dd3a998ca3ed86195a9d`  
		Last Modified: Wed, 10 Aug 2022 06:19:28 GMT  
		Size: 1.2 MB (1176360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458775e44b7b881bad4eb74564e5d89bf1a652b0a6139b393470e3947511522`  
		Last Modified: Wed, 10 Aug 2022 06:19:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ef260a1ad1352465c56c4f64504134432b8d3d143338c3e3f1d28b4baa38c6c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124362245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cdcf841b6257118f75389e3e0e2aa3be06c392d0847687846d270d30cfeeab`
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
# Tue, 09 Aug 2022 18:49:40 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:51:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:51:26 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:51:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:51:27 GMT
WORKDIR /go
# Wed, 10 Aug 2022 08:14:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 08:14:21 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 08:14:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 08:14:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 08:14:22 GMT
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
	-	`sha256:370520e38e9ed965c5d2cd2daaf4431f1d2a9806663edc24c91e7137673ddcbc`  
		Last Modified: Tue, 09 Aug 2022 18:56:17 GMT  
		Size: 113.2 MB (113190080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcdedfdcc75de69b3488999d0229cde87827f3a07d2a8f28e869413f71bd5c4`  
		Last Modified: Tue, 09 Aug 2022 18:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848bc4e4bc8147cbd275c615d51ec5163fbc2b82705ed1bba9ef58237b93bf1d`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 7.1 MB (7052782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5214650dd00d68f62fb6dd06529a360c4a2c6c24185c341b9f880d91ef775438`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e086fc28f8c601de8cdf5365d27a0ae8546d116fcf03e99d3b823bac7f9047`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:3b555cc203ac7475dc91c4b5d1b4a608f932ef4cd2cc5f28d4b0cafd12d0d8c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
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
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
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
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
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
$ docker pull caddy@sha256:04275786ace772b2bd49b3be4c692739aa6e3912b7cee35ac3e25dae660fba4a
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
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:bf37b595db36a904158da15138010561a6e121052e21f56aacbcc3cdf36e50c2
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
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:bb4ffc190f522d40ab390008e988db6e281e629e2363deb7e741a012d46d6488
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
$ docker pull caddy@sha256:4f6505a47382b5dec53662e2690f8f2c92c421c3183d6eadc0a2813923a33654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126629543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce17ec8cd808074c0b242c463275fec3b0882f6e530f6697c7c144b944d365d`
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
# Tue, 09 Aug 2022 19:15:05 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:16:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:16:41 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:16:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:16:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:16:42 GMT
WORKDIR /go
# Wed, 10 Aug 2022 02:26:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 02:26:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 02:26:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 02:26:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 02:26:07 GMT
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
	-	`sha256:af72e8bb74dba7b7a51456e414ac4999ff55a6a68e532a7cd1b6f32707be625f`  
		Last Modified: Tue, 09 Aug 2022 19:21:02 GMT  
		Size: 115.3 MB (115307225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421caacf35538ce671745cb9396eea38bf42cd3093eaf78dbcbe8bf5f83f82`  
		Last Modified: Tue, 09 Aug 2022 19:20:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06697ac7525490322e188b4b7c69500be186a38b1e83fc958cc4867577c89158`  
		Last Modified: Wed, 10 Aug 2022 02:26:41 GMT  
		Size: 6.9 MB (6941419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5272157df3949dde928ea90eaa0635d68c0e26b948696969f0ba100479f29d`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 1.3 MB (1289405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b2b76ccc7cb5ba98c8767f67ac01f45277649a0811109b81e23a55f84b2a5c`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e0bf3bb2f59bf72edcc69c72a3f95c05cae17d0dec32c3d2cdab3fd6fb45f6d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122605921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b23231332ede1e79114d2bcb35b96798016a2d8f1a3a5982908b631f73fc78a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 16:49:24 GMT
RUN apk add --no-cache ca-certificates
# Mon, 01 Aug 2022 16:49:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 16:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:04:45 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:13:52 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:13:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:13:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:13:53 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:53:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:53:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:53:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:53:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6060c9d5374931abb20ecd8e9328461917403d9561724f3df09c7e3fc87e8d7d`  
		Last Modified: Mon, 01 Aug 2022 17:33:54 GMT  
		Size: 284.7 KB (284743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc4259925cc07fecc6dc2421bf221853fe7ba33c4e1e630be41c927f23d5c05`  
		Last Modified: Mon, 01 Aug 2022 17:33:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42697db054e71ef6e42dc53a7b6145ae161eec6b80ac859c94ea018d09946540`  
		Last Modified: Mon, 01 Aug 2022 17:35:37 GMT  
		Size: 111.7 MB (111676715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc53c3f06fa91cdb79713efceaac7e9827d7848ed8c57d7fda971c1600072b6`  
		Last Modified: Mon, 01 Aug 2022 17:35:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020874bca98f79f6a60a6924e96c8fdf2ca45b4b3c0db0dea618c8e3d8c18ba`  
		Last Modified: Mon, 01 Aug 2022 17:54:26 GMT  
		Size: 6.8 MB (6808158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603ca030f2449d834b67ff449623a1cc9bb19d714d73c871eb89d39128826cfa`  
		Last Modified: Mon, 01 Aug 2022 17:54:25 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1699d137e1da0fc21e7af9c97fb58dd7c2e308a696d3669504d8ea4a2f9e62`  
		Last Modified: Mon, 01 Aug 2022 17:54:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bfa292826e8a20c33c3bf5175a0a10856b37d2fdf8a5ea891afbb9f863a1f13a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121428778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a30fdc400c6c38966a73f29da6af28b7751f8b2198b179292c2337837bdb884`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:59:34 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:08:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:08:40 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:08:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:54:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:54:18 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:54:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:54:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:54:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21b88218f56922c09b90952709a63bdecdde1ad2b4862aa7a697bbc578fecc`  
		Last Modified: Mon, 01 Aug 2022 17:35:21 GMT  
		Size: 111.4 MB (111449451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80adfea5b864e9bad4d701d93f87eedc3d89d7f508bdca67c613fdd65f46a1`  
		Last Modified: Mon, 01 Aug 2022 17:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134dbd094d15baa4d9e81748348ff6846c5d408a0fa5c195ae63f1e358ccdb`  
		Last Modified: Mon, 01 Aug 2022 17:54:58 GMT  
		Size: 6.1 MB (6067302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a36468cc7f395bc290ce04c2216468804fa13342fe0a49779a055958e9cb4c4`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 1.2 MB (1228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b67e6165d74b155d0ffc5f7a4cc9990cba565802b8ed0c9d754c3fb1ccffa2`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd8f1bce5198290bc50b08a93155ac38199a9dae48210ccfd5a4a41f5a95e19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121553906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ba051875de5f211ec4507df16e581228bf4219831d0589611b865a52455e5`
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
# Tue, 09 Aug 2022 19:11:57 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:13:28 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:13:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:13:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:13:31 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:52:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:52:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:52:15 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:52:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:52:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:52:20 GMT
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
	-	`sha256:cea4debaad2864fd0099780f6208841dc3a80054b81f7531944737f0f633e22a`  
		Last Modified: Tue, 09 Aug 2022 19:18:08 GMT  
		Size: 110.3 MB (110319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316bf57efd3b0cdd0835f8d3393e898cd27ed09707eff97189df62f132805299`  
		Last Modified: Tue, 09 Aug 2022 19:17:51 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a06f48c9f0345985d2098cac6d089f1580a8d87b4a2a782eb7bfbee426aef`  
		Last Modified: Wed, 10 Aug 2022 06:52:52 GMT  
		Size: 7.1 MB (7052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8265fec039b8677f92210d7029a762398511c9280be7d4d0efc1cb10be17d`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 1.2 MB (1189008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb8a803f3f8d02849a88c0ce723f1c41d644bba7cb86e8a8cf77a0ad559083e`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f17a6fc6ee71b48c6ad47db82361ca9e27fa68f51051efe89a989043228eca84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122067226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5d604a3361c5c0060249fcfc23e6dfa6eac3e105171f0a9c69e1f00e634c1`
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
# Tue, 09 Aug 2022 18:21:28 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:24:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:24:15 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:24:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:24:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:24:16 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:18:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:18:49 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:18:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:18:52 GMT
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
	-	`sha256:cf877b37b50b5ec020497c8c6cacab5479917d459e740c6380a0a14425d6ab8f`  
		Last Modified: Tue, 09 Aug 2022 18:30:52 GMT  
		Size: 110.3 MB (110317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15924e03aa834b25daf0b7536184d4b2e54a7463f9410eaca0d81764df5c962`  
		Last Modified: Tue, 09 Aug 2022 18:30:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70115b37e266a1fa2567feb847cdccaa6a8b04ef98c4fbe797713b9801bb31be`  
		Last Modified: Wed, 10 Aug 2022 06:19:29 GMT  
		Size: 7.5 MB (7482240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae18e224805e17c6354f387924797ff18689005d909dd3a998ca3ed86195a9d`  
		Last Modified: Wed, 10 Aug 2022 06:19:28 GMT  
		Size: 1.2 MB (1176360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458775e44b7b881bad4eb74564e5d89bf1a652b0a6139b393470e3947511522`  
		Last Modified: Wed, 10 Aug 2022 06:19:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ef260a1ad1352465c56c4f64504134432b8d3d143338c3e3f1d28b4baa38c6c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124362245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cdcf841b6257118f75389e3e0e2aa3be06c392d0847687846d270d30cfeeab`
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
# Tue, 09 Aug 2022 18:49:40 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:51:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:51:26 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:51:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:51:27 GMT
WORKDIR /go
# Wed, 10 Aug 2022 08:14:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 08:14:21 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 08:14:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 08:14:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 08:14:22 GMT
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
	-	`sha256:370520e38e9ed965c5d2cd2daaf4431f1d2a9806663edc24c91e7137673ddcbc`  
		Last Modified: Tue, 09 Aug 2022 18:56:17 GMT  
		Size: 113.2 MB (113190080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcdedfdcc75de69b3488999d0229cde87827f3a07d2a8f28e869413f71bd5c4`  
		Last Modified: Tue, 09 Aug 2022 18:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848bc4e4bc8147cbd275c615d51ec5163fbc2b82705ed1bba9ef58237b93bf1d`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 7.1 MB (7052782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5214650dd00d68f62fb6dd06529a360c4a2c6c24185c341b9f880d91ef775438`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e086fc28f8c601de8cdf5365d27a0ae8546d116fcf03e99d3b823bac7f9047`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 405.0 B  
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

### `caddy:2.5.2-builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
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
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
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
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-alpine`

```console
$ docker pull caddy@sha256:909a8efd2efb13ed2cd838b6c396e22e10b70018d9a4d332c28fa1079402e9c5
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
$ docker pull caddy@sha256:4f6505a47382b5dec53662e2690f8f2c92c421c3183d6eadc0a2813923a33654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126629543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce17ec8cd808074c0b242c463275fec3b0882f6e530f6697c7c144b944d365d`
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
# Tue, 09 Aug 2022 19:15:05 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:16:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:16:41 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:16:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:16:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:16:42 GMT
WORKDIR /go
# Wed, 10 Aug 2022 02:26:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 02:26:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 02:26:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 02:26:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 02:26:07 GMT
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
	-	`sha256:af72e8bb74dba7b7a51456e414ac4999ff55a6a68e532a7cd1b6f32707be625f`  
		Last Modified: Tue, 09 Aug 2022 19:21:02 GMT  
		Size: 115.3 MB (115307225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421caacf35538ce671745cb9396eea38bf42cd3093eaf78dbcbe8bf5f83f82`  
		Last Modified: Tue, 09 Aug 2022 19:20:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06697ac7525490322e188b4b7c69500be186a38b1e83fc958cc4867577c89158`  
		Last Modified: Wed, 10 Aug 2022 02:26:41 GMT  
		Size: 6.9 MB (6941419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5272157df3949dde928ea90eaa0635d68c0e26b948696969f0ba100479f29d`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 1.3 MB (1289405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b2b76ccc7cb5ba98c8767f67ac01f45277649a0811109b81e23a55f84b2a5c`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e0bf3bb2f59bf72edcc69c72a3f95c05cae17d0dec32c3d2cdab3fd6fb45f6d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122605921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b23231332ede1e79114d2bcb35b96798016a2d8f1a3a5982908b631f73fc78a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 16:49:24 GMT
RUN apk add --no-cache ca-certificates
# Mon, 01 Aug 2022 16:49:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 16:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:04:45 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:13:52 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:13:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:13:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:13:53 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:53:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:53:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:53:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:53:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6060c9d5374931abb20ecd8e9328461917403d9561724f3df09c7e3fc87e8d7d`  
		Last Modified: Mon, 01 Aug 2022 17:33:54 GMT  
		Size: 284.7 KB (284743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc4259925cc07fecc6dc2421bf221853fe7ba33c4e1e630be41c927f23d5c05`  
		Last Modified: Mon, 01 Aug 2022 17:33:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42697db054e71ef6e42dc53a7b6145ae161eec6b80ac859c94ea018d09946540`  
		Last Modified: Mon, 01 Aug 2022 17:35:37 GMT  
		Size: 111.7 MB (111676715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc53c3f06fa91cdb79713efceaac7e9827d7848ed8c57d7fda971c1600072b6`  
		Last Modified: Mon, 01 Aug 2022 17:35:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020874bca98f79f6a60a6924e96c8fdf2ca45b4b3c0db0dea618c8e3d8c18ba`  
		Last Modified: Mon, 01 Aug 2022 17:54:26 GMT  
		Size: 6.8 MB (6808158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603ca030f2449d834b67ff449623a1cc9bb19d714d73c871eb89d39128826cfa`  
		Last Modified: Mon, 01 Aug 2022 17:54:25 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1699d137e1da0fc21e7af9c97fb58dd7c2e308a696d3669504d8ea4a2f9e62`  
		Last Modified: Mon, 01 Aug 2022 17:54:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bfa292826e8a20c33c3bf5175a0a10856b37d2fdf8a5ea891afbb9f863a1f13a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121428778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a30fdc400c6c38966a73f29da6af28b7751f8b2198b179292c2337837bdb884`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:59:34 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:08:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:08:40 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:08:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:54:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:54:18 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:54:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:54:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:54:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21b88218f56922c09b90952709a63bdecdde1ad2b4862aa7a697bbc578fecc`  
		Last Modified: Mon, 01 Aug 2022 17:35:21 GMT  
		Size: 111.4 MB (111449451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80adfea5b864e9bad4d701d93f87eedc3d89d7f508bdca67c613fdd65f46a1`  
		Last Modified: Mon, 01 Aug 2022 17:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134dbd094d15baa4d9e81748348ff6846c5d408a0fa5c195ae63f1e358ccdb`  
		Last Modified: Mon, 01 Aug 2022 17:54:58 GMT  
		Size: 6.1 MB (6067302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a36468cc7f395bc290ce04c2216468804fa13342fe0a49779a055958e9cb4c4`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 1.2 MB (1228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b67e6165d74b155d0ffc5f7a4cc9990cba565802b8ed0c9d754c3fb1ccffa2`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd8f1bce5198290bc50b08a93155ac38199a9dae48210ccfd5a4a41f5a95e19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121553906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ba051875de5f211ec4507df16e581228bf4219831d0589611b865a52455e5`
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
# Tue, 09 Aug 2022 19:11:57 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:13:28 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:13:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:13:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:13:31 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:52:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:52:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:52:15 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:52:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:52:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:52:20 GMT
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
	-	`sha256:cea4debaad2864fd0099780f6208841dc3a80054b81f7531944737f0f633e22a`  
		Last Modified: Tue, 09 Aug 2022 19:18:08 GMT  
		Size: 110.3 MB (110319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316bf57efd3b0cdd0835f8d3393e898cd27ed09707eff97189df62f132805299`  
		Last Modified: Tue, 09 Aug 2022 19:17:51 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a06f48c9f0345985d2098cac6d089f1580a8d87b4a2a782eb7bfbee426aef`  
		Last Modified: Wed, 10 Aug 2022 06:52:52 GMT  
		Size: 7.1 MB (7052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8265fec039b8677f92210d7029a762398511c9280be7d4d0efc1cb10be17d`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 1.2 MB (1189008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb8a803f3f8d02849a88c0ce723f1c41d644bba7cb86e8a8cf77a0ad559083e`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f17a6fc6ee71b48c6ad47db82361ca9e27fa68f51051efe89a989043228eca84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122067226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5d604a3361c5c0060249fcfc23e6dfa6eac3e105171f0a9c69e1f00e634c1`
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
# Tue, 09 Aug 2022 18:21:28 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:24:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:24:15 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:24:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:24:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:24:16 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:18:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:18:49 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:18:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:18:52 GMT
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
	-	`sha256:cf877b37b50b5ec020497c8c6cacab5479917d459e740c6380a0a14425d6ab8f`  
		Last Modified: Tue, 09 Aug 2022 18:30:52 GMT  
		Size: 110.3 MB (110317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15924e03aa834b25daf0b7536184d4b2e54a7463f9410eaca0d81764df5c962`  
		Last Modified: Tue, 09 Aug 2022 18:30:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70115b37e266a1fa2567feb847cdccaa6a8b04ef98c4fbe797713b9801bb31be`  
		Last Modified: Wed, 10 Aug 2022 06:19:29 GMT  
		Size: 7.5 MB (7482240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae18e224805e17c6354f387924797ff18689005d909dd3a998ca3ed86195a9d`  
		Last Modified: Wed, 10 Aug 2022 06:19:28 GMT  
		Size: 1.2 MB (1176360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458775e44b7b881bad4eb74564e5d89bf1a652b0a6139b393470e3947511522`  
		Last Modified: Wed, 10 Aug 2022 06:19:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ef260a1ad1352465c56c4f64504134432b8d3d143338c3e3f1d28b4baa38c6c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124362245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cdcf841b6257118f75389e3e0e2aa3be06c392d0847687846d270d30cfeeab`
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
# Tue, 09 Aug 2022 18:49:40 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:51:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:51:26 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:51:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:51:27 GMT
WORKDIR /go
# Wed, 10 Aug 2022 08:14:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 08:14:21 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 08:14:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 08:14:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 08:14:22 GMT
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
	-	`sha256:370520e38e9ed965c5d2cd2daaf4431f1d2a9806663edc24c91e7137673ddcbc`  
		Last Modified: Tue, 09 Aug 2022 18:56:17 GMT  
		Size: 113.2 MB (113190080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcdedfdcc75de69b3488999d0229cde87827f3a07d2a8f28e869413f71bd5c4`  
		Last Modified: Tue, 09 Aug 2022 18:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848bc4e4bc8147cbd275c615d51ec5163fbc2b82705ed1bba9ef58237b93bf1d`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 7.1 MB (7052782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5214650dd00d68f62fb6dd06529a360c4a2c6c24185c341b9f880d91ef775438`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e086fc28f8c601de8cdf5365d27a0ae8546d116fcf03e99d3b823bac7f9047`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:3b555cc203ac7475dc91c4b5d1b4a608f932ef4cd2cc5f28d4b0cafd12d0d8c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:2.5.2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
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
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
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
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
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
$ docker pull caddy@sha256:bf37b595db36a904158da15138010561a6e121052e21f56aacbcc3cdf36e50c2
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
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:bb4ffc190f522d40ab390008e988db6e281e629e2363deb7e741a012d46d6488
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
$ docker pull caddy@sha256:4f6505a47382b5dec53662e2690f8f2c92c421c3183d6eadc0a2813923a33654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126629543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce17ec8cd808074c0b242c463275fec3b0882f6e530f6697c7c144b944d365d`
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
# Tue, 09 Aug 2022 19:15:05 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:16:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:16:41 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:16:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:16:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:16:42 GMT
WORKDIR /go
# Wed, 10 Aug 2022 02:26:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 02:26:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 02:26:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 02:26:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 02:26:07 GMT
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
	-	`sha256:af72e8bb74dba7b7a51456e414ac4999ff55a6a68e532a7cd1b6f32707be625f`  
		Last Modified: Tue, 09 Aug 2022 19:21:02 GMT  
		Size: 115.3 MB (115307225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421caacf35538ce671745cb9396eea38bf42cd3093eaf78dbcbe8bf5f83f82`  
		Last Modified: Tue, 09 Aug 2022 19:20:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06697ac7525490322e188b4b7c69500be186a38b1e83fc958cc4867577c89158`  
		Last Modified: Wed, 10 Aug 2022 02:26:41 GMT  
		Size: 6.9 MB (6941419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5272157df3949dde928ea90eaa0635d68c0e26b948696969f0ba100479f29d`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 1.3 MB (1289405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b2b76ccc7cb5ba98c8767f67ac01f45277649a0811109b81e23a55f84b2a5c`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e0bf3bb2f59bf72edcc69c72a3f95c05cae17d0dec32c3d2cdab3fd6fb45f6d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122605921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b23231332ede1e79114d2bcb35b96798016a2d8f1a3a5982908b631f73fc78a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 16:49:24 GMT
RUN apk add --no-cache ca-certificates
# Mon, 01 Aug 2022 16:49:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 16:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:04:45 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:13:52 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:13:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:13:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:13:53 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:53:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:53:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:53:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:53:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6060c9d5374931abb20ecd8e9328461917403d9561724f3df09c7e3fc87e8d7d`  
		Last Modified: Mon, 01 Aug 2022 17:33:54 GMT  
		Size: 284.7 KB (284743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc4259925cc07fecc6dc2421bf221853fe7ba33c4e1e630be41c927f23d5c05`  
		Last Modified: Mon, 01 Aug 2022 17:33:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42697db054e71ef6e42dc53a7b6145ae161eec6b80ac859c94ea018d09946540`  
		Last Modified: Mon, 01 Aug 2022 17:35:37 GMT  
		Size: 111.7 MB (111676715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc53c3f06fa91cdb79713efceaac7e9827d7848ed8c57d7fda971c1600072b6`  
		Last Modified: Mon, 01 Aug 2022 17:35:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020874bca98f79f6a60a6924e96c8fdf2ca45b4b3c0db0dea618c8e3d8c18ba`  
		Last Modified: Mon, 01 Aug 2022 17:54:26 GMT  
		Size: 6.8 MB (6808158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603ca030f2449d834b67ff449623a1cc9bb19d714d73c871eb89d39128826cfa`  
		Last Modified: Mon, 01 Aug 2022 17:54:25 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1699d137e1da0fc21e7af9c97fb58dd7c2e308a696d3669504d8ea4a2f9e62`  
		Last Modified: Mon, 01 Aug 2022 17:54:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bfa292826e8a20c33c3bf5175a0a10856b37d2fdf8a5ea891afbb9f863a1f13a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121428778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a30fdc400c6c38966a73f29da6af28b7751f8b2198b179292c2337837bdb884`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:59:34 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:08:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:08:40 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:08:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:54:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:54:18 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:54:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:54:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:54:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21b88218f56922c09b90952709a63bdecdde1ad2b4862aa7a697bbc578fecc`  
		Last Modified: Mon, 01 Aug 2022 17:35:21 GMT  
		Size: 111.4 MB (111449451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80adfea5b864e9bad4d701d93f87eedc3d89d7f508bdca67c613fdd65f46a1`  
		Last Modified: Mon, 01 Aug 2022 17:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134dbd094d15baa4d9e81748348ff6846c5d408a0fa5c195ae63f1e358ccdb`  
		Last Modified: Mon, 01 Aug 2022 17:54:58 GMT  
		Size: 6.1 MB (6067302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a36468cc7f395bc290ce04c2216468804fa13342fe0a49779a055958e9cb4c4`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 1.2 MB (1228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b67e6165d74b155d0ffc5f7a4cc9990cba565802b8ed0c9d754c3fb1ccffa2`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd8f1bce5198290bc50b08a93155ac38199a9dae48210ccfd5a4a41f5a95e19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121553906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ba051875de5f211ec4507df16e581228bf4219831d0589611b865a52455e5`
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
# Tue, 09 Aug 2022 19:11:57 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:13:28 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:13:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:13:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:13:31 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:52:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:52:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:52:15 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:52:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:52:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:52:20 GMT
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
	-	`sha256:cea4debaad2864fd0099780f6208841dc3a80054b81f7531944737f0f633e22a`  
		Last Modified: Tue, 09 Aug 2022 19:18:08 GMT  
		Size: 110.3 MB (110319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316bf57efd3b0cdd0835f8d3393e898cd27ed09707eff97189df62f132805299`  
		Last Modified: Tue, 09 Aug 2022 19:17:51 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a06f48c9f0345985d2098cac6d089f1580a8d87b4a2a782eb7bfbee426aef`  
		Last Modified: Wed, 10 Aug 2022 06:52:52 GMT  
		Size: 7.1 MB (7052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8265fec039b8677f92210d7029a762398511c9280be7d4d0efc1cb10be17d`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 1.2 MB (1189008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb8a803f3f8d02849a88c0ce723f1c41d644bba7cb86e8a8cf77a0ad559083e`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f17a6fc6ee71b48c6ad47db82361ca9e27fa68f51051efe89a989043228eca84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122067226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5d604a3361c5c0060249fcfc23e6dfa6eac3e105171f0a9c69e1f00e634c1`
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
# Tue, 09 Aug 2022 18:21:28 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:24:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:24:15 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:24:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:24:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:24:16 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:18:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:18:49 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:18:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:18:52 GMT
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
	-	`sha256:cf877b37b50b5ec020497c8c6cacab5479917d459e740c6380a0a14425d6ab8f`  
		Last Modified: Tue, 09 Aug 2022 18:30:52 GMT  
		Size: 110.3 MB (110317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15924e03aa834b25daf0b7536184d4b2e54a7463f9410eaca0d81764df5c962`  
		Last Modified: Tue, 09 Aug 2022 18:30:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70115b37e266a1fa2567feb847cdccaa6a8b04ef98c4fbe797713b9801bb31be`  
		Last Modified: Wed, 10 Aug 2022 06:19:29 GMT  
		Size: 7.5 MB (7482240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae18e224805e17c6354f387924797ff18689005d909dd3a998ca3ed86195a9d`  
		Last Modified: Wed, 10 Aug 2022 06:19:28 GMT  
		Size: 1.2 MB (1176360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458775e44b7b881bad4eb74564e5d89bf1a652b0a6139b393470e3947511522`  
		Last Modified: Wed, 10 Aug 2022 06:19:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:ef260a1ad1352465c56c4f64504134432b8d3d143338c3e3f1d28b4baa38c6c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124362245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cdcf841b6257118f75389e3e0e2aa3be06c392d0847687846d270d30cfeeab`
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
# Tue, 09 Aug 2022 18:49:40 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:51:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:51:26 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:51:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:51:27 GMT
WORKDIR /go
# Wed, 10 Aug 2022 08:14:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 08:14:21 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 08:14:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 08:14:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 08:14:22 GMT
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
	-	`sha256:370520e38e9ed965c5d2cd2daaf4431f1d2a9806663edc24c91e7137673ddcbc`  
		Last Modified: Tue, 09 Aug 2022 18:56:17 GMT  
		Size: 113.2 MB (113190080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcdedfdcc75de69b3488999d0229cde87827f3a07d2a8f28e869413f71bd5c4`  
		Last Modified: Tue, 09 Aug 2022 18:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848bc4e4bc8147cbd275c615d51ec5163fbc2b82705ed1bba9ef58237b93bf1d`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 7.1 MB (7052782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5214650dd00d68f62fb6dd06529a360c4a2c6c24185c341b9f880d91ef775438`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e086fc28f8c601de8cdf5365d27a0ae8546d116fcf03e99d3b823bac7f9047`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 405.0 B  
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

### `caddy:builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
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
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
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
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:909a8efd2efb13ed2cd838b6c396e22e10b70018d9a4d332c28fa1079402e9c5
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
$ docker pull caddy@sha256:4f6505a47382b5dec53662e2690f8f2c92c421c3183d6eadc0a2813923a33654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126629543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce17ec8cd808074c0b242c463275fec3b0882f6e530f6697c7c144b944d365d`
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
# Tue, 09 Aug 2022 19:15:05 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:16:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:16:41 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:16:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:16:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:16:42 GMT
WORKDIR /go
# Wed, 10 Aug 2022 02:26:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 02:26:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:26:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 02:26:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 02:26:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 02:26:07 GMT
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
	-	`sha256:af72e8bb74dba7b7a51456e414ac4999ff55a6a68e532a7cd1b6f32707be625f`  
		Last Modified: Tue, 09 Aug 2022 19:21:02 GMT  
		Size: 115.3 MB (115307225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a421caacf35538ce671745cb9396eea38bf42cd3093eaf78dbcbe8bf5f83f82`  
		Last Modified: Tue, 09 Aug 2022 19:20:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06697ac7525490322e188b4b7c69500be186a38b1e83fc958cc4867577c89158`  
		Last Modified: Wed, 10 Aug 2022 02:26:41 GMT  
		Size: 6.9 MB (6941419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5272157df3949dde928ea90eaa0635d68c0e26b948696969f0ba100479f29d`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 1.3 MB (1289405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b2b76ccc7cb5ba98c8767f67ac01f45277649a0811109b81e23a55f84b2a5c`  
		Last Modified: Wed, 10 Aug 2022 02:26:40 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e0bf3bb2f59bf72edcc69c72a3f95c05cae17d0dec32c3d2cdab3fd6fb45f6d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122605921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b23231332ede1e79114d2bcb35b96798016a2d8f1a3a5982908b631f73fc78a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 16:49:24 GMT
RUN apk add --no-cache ca-certificates
# Mon, 01 Aug 2022 16:49:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 16:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:04:45 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:13:52 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:13:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:13:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:13:53 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:53:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:53:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:53:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:53:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6060c9d5374931abb20ecd8e9328461917403d9561724f3df09c7e3fc87e8d7d`  
		Last Modified: Mon, 01 Aug 2022 17:33:54 GMT  
		Size: 284.7 KB (284743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc4259925cc07fecc6dc2421bf221853fe7ba33c4e1e630be41c927f23d5c05`  
		Last Modified: Mon, 01 Aug 2022 17:33:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42697db054e71ef6e42dc53a7b6145ae161eec6b80ac859c94ea018d09946540`  
		Last Modified: Mon, 01 Aug 2022 17:35:37 GMT  
		Size: 111.7 MB (111676715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc53c3f06fa91cdb79713efceaac7e9827d7848ed8c57d7fda971c1600072b6`  
		Last Modified: Mon, 01 Aug 2022 17:35:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020874bca98f79f6a60a6924e96c8fdf2ca45b4b3c0db0dea618c8e3d8c18ba`  
		Last Modified: Mon, 01 Aug 2022 17:54:26 GMT  
		Size: 6.8 MB (6808158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603ca030f2449d834b67ff449623a1cc9bb19d714d73c871eb89d39128826cfa`  
		Last Modified: Mon, 01 Aug 2022 17:54:25 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1699d137e1da0fc21e7af9c97fb58dd7c2e308a696d3669504d8ea4a2f9e62`  
		Last Modified: Mon, 01 Aug 2022 17:54:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bfa292826e8a20c33c3bf5175a0a10856b37d2fdf8a5ea891afbb9f863a1f13a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121428778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a30fdc400c6c38966a73f29da6af28b7751f8b2198b179292c2337837bdb884`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:59:34 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 17:08:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 17:08:40 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 17:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 17:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 17:08:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:54:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:54:18 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:54:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:54:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:54:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:54:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21b88218f56922c09b90952709a63bdecdde1ad2b4862aa7a697bbc578fecc`  
		Last Modified: Mon, 01 Aug 2022 17:35:21 GMT  
		Size: 111.4 MB (111449451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80adfea5b864e9bad4d701d93f87eedc3d89d7f508bdca67c613fdd65f46a1`  
		Last Modified: Mon, 01 Aug 2022 17:34:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2134dbd094d15baa4d9e81748348ff6846c5d408a0fa5c195ae63f1e358ccdb`  
		Last Modified: Mon, 01 Aug 2022 17:54:58 GMT  
		Size: 6.1 MB (6067302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a36468cc7f395bc290ce04c2216468804fa13342fe0a49779a055958e9cb4c4`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 1.2 MB (1228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b67e6165d74b155d0ffc5f7a4cc9990cba565802b8ed0c9d754c3fb1ccffa2`  
		Last Modified: Mon, 01 Aug 2022 17:54:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd8f1bce5198290bc50b08a93155ac38199a9dae48210ccfd5a4a41f5a95e19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121553906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ba051875de5f211ec4507df16e581228bf4219831d0589611b865a52455e5`
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
# Tue, 09 Aug 2022 19:11:57 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 19:13:28 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 19:13:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 19:13:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 19:13:31 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:52:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:52:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:52:15 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:52:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:52:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:52:20 GMT
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
	-	`sha256:cea4debaad2864fd0099780f6208841dc3a80054b81f7531944737f0f633e22a`  
		Last Modified: Tue, 09 Aug 2022 19:18:08 GMT  
		Size: 110.3 MB (110319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316bf57efd3b0cdd0835f8d3393e898cd27ed09707eff97189df62f132805299`  
		Last Modified: Tue, 09 Aug 2022 19:17:51 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a06f48c9f0345985d2098cac6d089f1580a8d87b4a2a782eb7bfbee426aef`  
		Last Modified: Wed, 10 Aug 2022 06:52:52 GMT  
		Size: 7.1 MB (7052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8265fec039b8677f92210d7029a762398511c9280be7d4d0efc1cb10be17d`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 1.2 MB (1189008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb8a803f3f8d02849a88c0ce723f1c41d644bba7cb86e8a8cf77a0ad559083e`  
		Last Modified: Wed, 10 Aug 2022 06:52:51 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f17a6fc6ee71b48c6ad47db82361ca9e27fa68f51051efe89a989043228eca84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122067226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5d604a3361c5c0060249fcfc23e6dfa6eac3e105171f0a9c69e1f00e634c1`
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
# Tue, 09 Aug 2022 18:21:28 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:24:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:24:15 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:24:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:24:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:24:16 GMT
WORKDIR /go
# Wed, 10 Aug 2022 06:18:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 06:18:49 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 06:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 06:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 06:18:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 06:18:52 GMT
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
	-	`sha256:cf877b37b50b5ec020497c8c6cacab5479917d459e740c6380a0a14425d6ab8f`  
		Last Modified: Tue, 09 Aug 2022 18:30:52 GMT  
		Size: 110.3 MB (110317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15924e03aa834b25daf0b7536184d4b2e54a7463f9410eaca0d81764df5c962`  
		Last Modified: Tue, 09 Aug 2022 18:30:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70115b37e266a1fa2567feb847cdccaa6a8b04ef98c4fbe797713b9801bb31be`  
		Last Modified: Wed, 10 Aug 2022 06:19:29 GMT  
		Size: 7.5 MB (7482240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae18e224805e17c6354f387924797ff18689005d909dd3a998ca3ed86195a9d`  
		Last Modified: Wed, 10 Aug 2022 06:19:28 GMT  
		Size: 1.2 MB (1176360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9458775e44b7b881bad4eb74564e5d89bf1a652b0a6139b393470e3947511522`  
		Last Modified: Wed, 10 Aug 2022 06:19:27 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ef260a1ad1352465c56c4f64504134432b8d3d143338c3e3f1d28b4baa38c6c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124362245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cdcf841b6257118f75389e3e0e2aa3be06c392d0847687846d270d30cfeeab`
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
# Tue, 09 Aug 2022 18:49:40 GMT
ENV GOLANG_VERSION=1.18.5
# Tue, 09 Aug 2022 18:51:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 09 Aug 2022 18:51:26 GMT
ENV GOPATH=/go
# Tue, 09 Aug 2022 18:51:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 18:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Aug 2022 18:51:27 GMT
WORKDIR /go
# Wed, 10 Aug 2022 08:14:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 10 Aug 2022 08:14:21 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 08:14:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Aug 2022 08:14:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 10 Aug 2022 08:14:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 10 Aug 2022 08:14:22 GMT
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
	-	`sha256:370520e38e9ed965c5d2cd2daaf4431f1d2a9806663edc24c91e7137673ddcbc`  
		Last Modified: Tue, 09 Aug 2022 18:56:17 GMT  
		Size: 113.2 MB (113190080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcdedfdcc75de69b3488999d0229cde87827f3a07d2a8f28e869413f71bd5c4`  
		Last Modified: Tue, 09 Aug 2022 18:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848bc4e4bc8147cbd275c615d51ec5163fbc2b82705ed1bba9ef58237b93bf1d`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 7.1 MB (7052782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5214650dd00d68f62fb6dd06529a360c4a2c6c24185c341b9f880d91ef775438`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e086fc28f8c601de8cdf5365d27a0ae8546d116fcf03e99d3b823bac7f9047`  
		Last Modified: Wed, 10 Aug 2022 08:15:36 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:3b555cc203ac7475dc91c4b5d1b4a608f932ef4cd2cc5f28d4b0cafd12d0d8c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
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
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
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
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:04275786ace772b2bd49b3be4c692739aa6e3912b7cee35ac3e25dae660fba4a
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
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
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
