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
$ docker pull caddy@sha256:c2aa034bd91237e02c80e030f1366fe0e20c88dfc6b9eac5c3cfefdc447b7bc9
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
$ docker pull caddy@sha256:cfa7d94aa1f0c68a167b147a8573711283df2cd6fc285d220387f20206ff4874
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83af79bf9e25fcac6c74f9e4862c41808daae08fc9693798b23edb747e6e938`
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
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:22 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:22 GMT
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
$ docker pull caddy@sha256:ab90c32af49182ef7512475520559c58882dc9c3eb856bd05045845355bf5b70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499d71de73836366f4be3ee44abf878f97102a0f242d2afb55a1238073b79b6`
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
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:21 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:21 GMT
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
$ docker pull caddy@sha256:7981b1b833894ee4cde9129ba6181dd80307b7e1df3ecd18b9720d88993e1c27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a985003f9f6cbce93bc66be158b0f622194e08f2b1ee5a8eba5cc793446602b`
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
# Wed, 07 Sep 2022 20:57:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:23 GMT
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
$ docker pull caddy@sha256:03f7dc5da8bd904d5942283fe31d401249560bb74b0dbfd88eba3c65e5ef9493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea1482cd071f0d18c0519a9b6819e949540f0e761ed8645f95060c4917f7c0`
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
# Wed, 07 Sep 2022 20:39:31 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:39:32 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:39:33 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:39:34 GMT
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
$ docker pull caddy@sha256:c98b27fc9159cf13c479d2052080ca25cfcbe5546cfe258c1a6f70827801f6e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d851d72b6e66e7190c29af3b6f08ff07e0372c054fbc46ae13ad4f38f9554e`
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
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:24 GMT
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
$ docker pull caddy@sha256:8147dd7b152004aa641f7699109649703831e18dc563fbb6448d54e88ef94766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7460051eff8773d7f2c072637754453656be2c21c74f71711669c5ab9bbba9`
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
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:28 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:29 GMT
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
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:b31ff95e98737b849d6af1fb9d9cb54a66ba3684564b3310541f60b12b1dd619
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
$ docker pull caddy@sha256:cfa7d94aa1f0c68a167b147a8573711283df2cd6fc285d220387f20206ff4874
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83af79bf9e25fcac6c74f9e4862c41808daae08fc9693798b23edb747e6e938`
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
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:22 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:22 GMT
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
$ docker pull caddy@sha256:ab90c32af49182ef7512475520559c58882dc9c3eb856bd05045845355bf5b70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499d71de73836366f4be3ee44abf878f97102a0f242d2afb55a1238073b79b6`
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
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:21 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:21 GMT
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
$ docker pull caddy@sha256:7981b1b833894ee4cde9129ba6181dd80307b7e1df3ecd18b9720d88993e1c27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a985003f9f6cbce93bc66be158b0f622194e08f2b1ee5a8eba5cc793446602b`
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
# Wed, 07 Sep 2022 20:57:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:23 GMT
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
$ docker pull caddy@sha256:03f7dc5da8bd904d5942283fe31d401249560bb74b0dbfd88eba3c65e5ef9493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea1482cd071f0d18c0519a9b6819e949540f0e761ed8645f95060c4917f7c0`
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
# Wed, 07 Sep 2022 20:39:31 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:39:32 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:39:33 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:39:34 GMT
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
$ docker pull caddy@sha256:c98b27fc9159cf13c479d2052080ca25cfcbe5546cfe258c1a6f70827801f6e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d851d72b6e66e7190c29af3b6f08ff07e0372c054fbc46ae13ad4f38f9554e`
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
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:24 GMT
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
$ docker pull caddy@sha256:8147dd7b152004aa641f7699109649703831e18dc563fbb6448d54e88ef94766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7460051eff8773d7f2c072637754453656be2c21c74f71711669c5ab9bbba9`
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
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:28 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:29 GMT
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
$ docker pull caddy@sha256:1a8f153ebe56283c4d5168d92c049b00ae1c635248f99295c4c106ccfad3012f
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

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:35d5468f9f5b642625cd0db6ac93f5fb012037c4783516a2db9ee1f9942a5f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126581869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446a17d6179d93d6f4f576b01e0d83b0271aae295f07c5e1fdb031f1af9bdbba`
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
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:25 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:27 GMT
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
	-	`sha256:39a0d8604657ba9022aa5b88de3771f9a87f7a100187743f8b02c4995137f7c7`  
		Last Modified: Wed, 07 Sep 2022 21:20:09 GMT  
		Size: 1.2 MB (1215200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf75964ac643c8e0de2048260f7080c9a9afd12c87c3f93305892303c02626`  
		Last Modified: Wed, 07 Sep 2022 21:20:08 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:52932e74f09f4f600395ef0e65ac7761f74590c784de385b329c3deba73e9728
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122585761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceffdb3edb815118e8e62d2de89c304f5c9789a479a4aa646137643225c71277`
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
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:30 GMT
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
	-	`sha256:714c3b82fd5725d5c508bf921d8e44a826b6e80b7cf80206371441629020f7df`  
		Last Modified: Wed, 07 Sep 2022 20:50:44 GMT  
		Size: 1.2 MB (1162989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b035ad2bb7133b1e1f29d51c79911610b64ce645964402e0303856cc02a489d6`  
		Last Modified: Wed, 07 Sep 2022 20:50:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d54381d61daa9bbeb03bcbaa1c9fbf5e4890cd3f23fc2aebc13bb763bcd78efe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121421388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2fbb736245edf10b20547bdda39806040da01b5ed7daad738d04767e91fd47`
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
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:57:33 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:57:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:57:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:57:35 GMT
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
	-	`sha256:068f91f2941da883f37d54e440827226340fd3cad687e8529e236e235400c098`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 1.2 MB (1159978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae346762b582e00a5f229e741b110848ff0c3b95a30e95e56d235d7eed3c31`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e4ced291a901313117012e281dd0de28ec1d3c2e70246002d0533aea698925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121532298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3045db8e0202ea02304fde36f24f2fa1f10473c6b30d8dd9cc85392b3e63eab`
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
# Wed, 07 Sep 2022 20:39:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:39:42 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:39:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:39:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:39:46 GMT
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
	-	`sha256:5340d2088ba2060ab6fd7ac03124f5c7f395a51670305bf90a89da96988e8daa`  
		Last Modified: Wed, 07 Sep 2022 20:41:12 GMT  
		Size: 1.1 MB (1120446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5c4ba17c8241ba8dfbe915956db306ef689730489ef97462e99e641a0c1bf`  
		Last Modified: Wed, 07 Sep 2022 20:41:11 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:2cc10ae309cb5fac54e5e8d39dbef0f535d8ad5336c9b32415250274fcc0cfb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122072737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8c0fd8624128c41541d92222a799f89ca10620bd3b187579c1c6cba4827192`
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
# Wed, 07 Sep 2022 21:16:31 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:32 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:16:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:16:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:16:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:16:35 GMT
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
	-	`sha256:fdb755156f20625cf7436ebf9dd3e9d73ed62942073cbc911c4f42e739412d51`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 1.1 MB (1103854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be64bd7379e703449226d281d2a47bfacaf4193e886ff12bd078fa95dd5823f`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ef06f5dd643bb6af248afc42b5a46c88c13404a0b8718cf9ab9e5b07a36e6c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b9e4f098357534de1347fdb9b83e146abab58747e67d367d7e39f967d47b3a`
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
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:41:37 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:41:38 GMT
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
	-	`sha256:b6163d00c71b4379b800d1de8c81291389a7c79cc6d574dcce5e37183b3afde4`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 1.2 MB (1167442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532161760fe5ac59a0240e62f0bc251ea4e8de1f539811850f43e3802394e34`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:7a5223f7720e5df685236b56c58dd57fad525b88fdb76e56e121a9e3be273615
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2494943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ea73be5cb10a5570dad83431d3aba123ed40e564b9f20fbf123f2be4546100`
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
# Wed, 07 Sep 2022 21:18:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:18:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:18:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:57 GMT
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
	-	`sha256:ff9d42bb565792710d4018b199ac636b9be0ffb9db23b35bc1eee69dca771c33`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61760b64ebc2bb823a7baca5dd0c0d7db3befbbed5ad1a8c1a5e6eaf346ca0b4`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f87d92375e5d9779ea8a646f053e96096f690a3c73617055f862f173f5033`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3271b3d777871daea415771bcf19be13bdf3d9fcd47e5c1777c9f480790716e`  
		Last Modified: Wed, 07 Sep 2022 21:27:15 GMT  
		Size: 1.9 MB (1868000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b438765ca79769b19f152009561021f6f8ac5c4446b1fc99e7fd9b10a4e8adba`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:1fb3a7ef40462a897a1a3b8ed772a24cfc804cd63942b33130cd129a188cccd2
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
$ docker pull caddy@sha256:35d5468f9f5b642625cd0db6ac93f5fb012037c4783516a2db9ee1f9942a5f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126581869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446a17d6179d93d6f4f576b01e0d83b0271aae295f07c5e1fdb031f1af9bdbba`
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
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:25 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:27 GMT
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
	-	`sha256:39a0d8604657ba9022aa5b88de3771f9a87f7a100187743f8b02c4995137f7c7`  
		Last Modified: Wed, 07 Sep 2022 21:20:09 GMT  
		Size: 1.2 MB (1215200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf75964ac643c8e0de2048260f7080c9a9afd12c87c3f93305892303c02626`  
		Last Modified: Wed, 07 Sep 2022 21:20:08 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:52932e74f09f4f600395ef0e65ac7761f74590c784de385b329c3deba73e9728
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122585761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceffdb3edb815118e8e62d2de89c304f5c9789a479a4aa646137643225c71277`
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
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:30 GMT
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
	-	`sha256:714c3b82fd5725d5c508bf921d8e44a826b6e80b7cf80206371441629020f7df`  
		Last Modified: Wed, 07 Sep 2022 20:50:44 GMT  
		Size: 1.2 MB (1162989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b035ad2bb7133b1e1f29d51c79911610b64ce645964402e0303856cc02a489d6`  
		Last Modified: Wed, 07 Sep 2022 20:50:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d54381d61daa9bbeb03bcbaa1c9fbf5e4890cd3f23fc2aebc13bb763bcd78efe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121421388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2fbb736245edf10b20547bdda39806040da01b5ed7daad738d04767e91fd47`
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
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:57:33 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:57:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:57:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:57:35 GMT
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
	-	`sha256:068f91f2941da883f37d54e440827226340fd3cad687e8529e236e235400c098`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 1.2 MB (1159978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae346762b582e00a5f229e741b110848ff0c3b95a30e95e56d235d7eed3c31`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e4ced291a901313117012e281dd0de28ec1d3c2e70246002d0533aea698925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121532298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3045db8e0202ea02304fde36f24f2fa1f10473c6b30d8dd9cc85392b3e63eab`
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
# Wed, 07 Sep 2022 20:39:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:39:42 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:39:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:39:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:39:46 GMT
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
	-	`sha256:5340d2088ba2060ab6fd7ac03124f5c7f395a51670305bf90a89da96988e8daa`  
		Last Modified: Wed, 07 Sep 2022 20:41:12 GMT  
		Size: 1.1 MB (1120446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5c4ba17c8241ba8dfbe915956db306ef689730489ef97462e99e641a0c1bf`  
		Last Modified: Wed, 07 Sep 2022 20:41:11 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:2cc10ae309cb5fac54e5e8d39dbef0f535d8ad5336c9b32415250274fcc0cfb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122072737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8c0fd8624128c41541d92222a799f89ca10620bd3b187579c1c6cba4827192`
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
# Wed, 07 Sep 2022 21:16:31 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:32 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:16:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:16:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:16:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:16:35 GMT
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
	-	`sha256:fdb755156f20625cf7436ebf9dd3e9d73ed62942073cbc911c4f42e739412d51`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 1.1 MB (1103854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be64bd7379e703449226d281d2a47bfacaf4193e886ff12bd078fa95dd5823f`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ef06f5dd643bb6af248afc42b5a46c88c13404a0b8718cf9ab9e5b07a36e6c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b9e4f098357534de1347fdb9b83e146abab58747e67d367d7e39f967d47b3a`
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
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:41:37 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:41:38 GMT
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
	-	`sha256:b6163d00c71b4379b800d1de8c81291389a7c79cc6d574dcce5e37183b3afde4`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 1.2 MB (1167442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532161760fe5ac59a0240e62f0bc251ea4e8de1f539811850f43e3802394e34`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fc7d6643b94f172dc0be1c2a55fe404556c0ef4308cd01485587e677fd69b58f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5bd4a15f1f1608bda512eef3fb6ab85a621321eaf331befc3460e95e84bbdfc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:7a5223f7720e5df685236b56c58dd57fad525b88fdb76e56e121a9e3be273615
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2494943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ea73be5cb10a5570dad83431d3aba123ed40e564b9f20fbf123f2be4546100`
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
# Wed, 07 Sep 2022 21:18:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:18:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:18:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:57 GMT
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
	-	`sha256:ff9d42bb565792710d4018b199ac636b9be0ffb9db23b35bc1eee69dca771c33`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61760b64ebc2bb823a7baca5dd0c0d7db3befbbed5ad1a8c1a5e6eaf346ca0b4`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f87d92375e5d9779ea8a646f053e96096f690a3c73617055f862f173f5033`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3271b3d777871daea415771bcf19be13bdf3d9fcd47e5c1777c9f480790716e`  
		Last Modified: Wed, 07 Sep 2022 21:27:15 GMT  
		Size: 1.9 MB (1868000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b438765ca79769b19f152009561021f6f8ac5c4446b1fc99e7fd9b10a4e8adba`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:e93223c9604a42ed32a365ac8f0a2cb429b636c5cd64417763033237d281936d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8e736a0201648378f698716a66fc532320d11f8357cb58773c47b5cfe6cfed3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e43f46a4015c9bdce6f65c400e02eca5ae6d1a642bfc498c1c231e8d60a8958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2`

```console
$ docker pull caddy@sha256:c2aa034bd91237e02c80e030f1366fe0e20c88dfc6b9eac5c3cfefdc447b7bc9
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
$ docker pull caddy@sha256:cfa7d94aa1f0c68a167b147a8573711283df2cd6fc285d220387f20206ff4874
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83af79bf9e25fcac6c74f9e4862c41808daae08fc9693798b23edb747e6e938`
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
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:22 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:22 GMT
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
$ docker pull caddy@sha256:ab90c32af49182ef7512475520559c58882dc9c3eb856bd05045845355bf5b70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499d71de73836366f4be3ee44abf878f97102a0f242d2afb55a1238073b79b6`
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
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:21 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:21 GMT
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
$ docker pull caddy@sha256:7981b1b833894ee4cde9129ba6181dd80307b7e1df3ecd18b9720d88993e1c27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a985003f9f6cbce93bc66be158b0f622194e08f2b1ee5a8eba5cc793446602b`
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
# Wed, 07 Sep 2022 20:57:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:23 GMT
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
$ docker pull caddy@sha256:03f7dc5da8bd904d5942283fe31d401249560bb74b0dbfd88eba3c65e5ef9493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea1482cd071f0d18c0519a9b6819e949540f0e761ed8645f95060c4917f7c0`
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
# Wed, 07 Sep 2022 20:39:31 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:39:32 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:39:33 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:39:34 GMT
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
$ docker pull caddy@sha256:c98b27fc9159cf13c479d2052080ca25cfcbe5546cfe258c1a6f70827801f6e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d851d72b6e66e7190c29af3b6f08ff07e0372c054fbc46ae13ad4f38f9554e`
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
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:24 GMT
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
$ docker pull caddy@sha256:8147dd7b152004aa641f7699109649703831e18dc563fbb6448d54e88ef94766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7460051eff8773d7f2c072637754453656be2c21c74f71711669c5ab9bbba9`
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
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:28 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:29 GMT
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
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-alpine`

```console
$ docker pull caddy@sha256:b31ff95e98737b849d6af1fb9d9cb54a66ba3684564b3310541f60b12b1dd619
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
$ docker pull caddy@sha256:cfa7d94aa1f0c68a167b147a8573711283df2cd6fc285d220387f20206ff4874
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83af79bf9e25fcac6c74f9e4862c41808daae08fc9693798b23edb747e6e938`
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
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:22 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:22 GMT
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
$ docker pull caddy@sha256:ab90c32af49182ef7512475520559c58882dc9c3eb856bd05045845355bf5b70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499d71de73836366f4be3ee44abf878f97102a0f242d2afb55a1238073b79b6`
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
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:21 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:21 GMT
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
$ docker pull caddy@sha256:7981b1b833894ee4cde9129ba6181dd80307b7e1df3ecd18b9720d88993e1c27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a985003f9f6cbce93bc66be158b0f622194e08f2b1ee5a8eba5cc793446602b`
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
# Wed, 07 Sep 2022 20:57:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:23 GMT
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
$ docker pull caddy@sha256:03f7dc5da8bd904d5942283fe31d401249560bb74b0dbfd88eba3c65e5ef9493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea1482cd071f0d18c0519a9b6819e949540f0e761ed8645f95060c4917f7c0`
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
# Wed, 07 Sep 2022 20:39:31 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:39:32 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:39:33 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:39:34 GMT
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
$ docker pull caddy@sha256:c98b27fc9159cf13c479d2052080ca25cfcbe5546cfe258c1a6f70827801f6e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d851d72b6e66e7190c29af3b6f08ff07e0372c054fbc46ae13ad4f38f9554e`
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
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:24 GMT
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
$ docker pull caddy@sha256:8147dd7b152004aa641f7699109649703831e18dc563fbb6448d54e88ef94766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7460051eff8773d7f2c072637754453656be2c21c74f71711669c5ab9bbba9`
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
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:28 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:29 GMT
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
$ docker pull caddy@sha256:1a8f153ebe56283c4d5168d92c049b00ae1c635248f99295c4c106ccfad3012f
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

### `caddy:2.5.2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:35d5468f9f5b642625cd0db6ac93f5fb012037c4783516a2db9ee1f9942a5f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126581869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446a17d6179d93d6f4f576b01e0d83b0271aae295f07c5e1fdb031f1af9bdbba`
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
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:25 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:27 GMT
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
	-	`sha256:39a0d8604657ba9022aa5b88de3771f9a87f7a100187743f8b02c4995137f7c7`  
		Last Modified: Wed, 07 Sep 2022 21:20:09 GMT  
		Size: 1.2 MB (1215200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf75964ac643c8e0de2048260f7080c9a9afd12c87c3f93305892303c02626`  
		Last Modified: Wed, 07 Sep 2022 21:20:08 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:52932e74f09f4f600395ef0e65ac7761f74590c784de385b329c3deba73e9728
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122585761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceffdb3edb815118e8e62d2de89c304f5c9789a479a4aa646137643225c71277`
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
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:30 GMT
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
	-	`sha256:714c3b82fd5725d5c508bf921d8e44a826b6e80b7cf80206371441629020f7df`  
		Last Modified: Wed, 07 Sep 2022 20:50:44 GMT  
		Size: 1.2 MB (1162989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b035ad2bb7133b1e1f29d51c79911610b64ce645964402e0303856cc02a489d6`  
		Last Modified: Wed, 07 Sep 2022 20:50:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d54381d61daa9bbeb03bcbaa1c9fbf5e4890cd3f23fc2aebc13bb763bcd78efe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121421388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2fbb736245edf10b20547bdda39806040da01b5ed7daad738d04767e91fd47`
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
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:57:33 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:57:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:57:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:57:35 GMT
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
	-	`sha256:068f91f2941da883f37d54e440827226340fd3cad687e8529e236e235400c098`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 1.2 MB (1159978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae346762b582e00a5f229e741b110848ff0c3b95a30e95e56d235d7eed3c31`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e4ced291a901313117012e281dd0de28ec1d3c2e70246002d0533aea698925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121532298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3045db8e0202ea02304fde36f24f2fa1f10473c6b30d8dd9cc85392b3e63eab`
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
# Wed, 07 Sep 2022 20:39:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:39:42 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:39:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:39:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:39:46 GMT
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
	-	`sha256:5340d2088ba2060ab6fd7ac03124f5c7f395a51670305bf90a89da96988e8daa`  
		Last Modified: Wed, 07 Sep 2022 20:41:12 GMT  
		Size: 1.1 MB (1120446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5c4ba17c8241ba8dfbe915956db306ef689730489ef97462e99e641a0c1bf`  
		Last Modified: Wed, 07 Sep 2022 20:41:11 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:2cc10ae309cb5fac54e5e8d39dbef0f535d8ad5336c9b32415250274fcc0cfb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122072737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8c0fd8624128c41541d92222a799f89ca10620bd3b187579c1c6cba4827192`
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
# Wed, 07 Sep 2022 21:16:31 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:32 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:16:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:16:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:16:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:16:35 GMT
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
	-	`sha256:fdb755156f20625cf7436ebf9dd3e9d73ed62942073cbc911c4f42e739412d51`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 1.1 MB (1103854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be64bd7379e703449226d281d2a47bfacaf4193e886ff12bd078fa95dd5823f`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ef06f5dd643bb6af248afc42b5a46c88c13404a0b8718cf9ab9e5b07a36e6c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b9e4f098357534de1347fdb9b83e146abab58747e67d367d7e39f967d47b3a`
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
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:41:37 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:41:38 GMT
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
	-	`sha256:b6163d00c71b4379b800d1de8c81291389a7c79cc6d574dcce5e37183b3afde4`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 1.2 MB (1167442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532161760fe5ac59a0240e62f0bc251ea4e8de1f539811850f43e3802394e34`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:7a5223f7720e5df685236b56c58dd57fad525b88fdb76e56e121a9e3be273615
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2494943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ea73be5cb10a5570dad83431d3aba123ed40e564b9f20fbf123f2be4546100`
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
# Wed, 07 Sep 2022 21:18:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:18:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:18:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:57 GMT
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
	-	`sha256:ff9d42bb565792710d4018b199ac636b9be0ffb9db23b35bc1eee69dca771c33`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61760b64ebc2bb823a7baca5dd0c0d7db3befbbed5ad1a8c1a5e6eaf346ca0b4`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f87d92375e5d9779ea8a646f053e96096f690a3c73617055f862f173f5033`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3271b3d777871daea415771bcf19be13bdf3d9fcd47e5c1777c9f480790716e`  
		Last Modified: Wed, 07 Sep 2022 21:27:15 GMT  
		Size: 1.9 MB (1868000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b438765ca79769b19f152009561021f6f8ac5c4446b1fc99e7fd9b10a4e8adba`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-alpine`

```console
$ docker pull caddy@sha256:1fb3a7ef40462a897a1a3b8ed772a24cfc804cd63942b33130cd129a188cccd2
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
$ docker pull caddy@sha256:35d5468f9f5b642625cd0db6ac93f5fb012037c4783516a2db9ee1f9942a5f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126581869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446a17d6179d93d6f4f576b01e0d83b0271aae295f07c5e1fdb031f1af9bdbba`
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
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:25 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:27 GMT
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
	-	`sha256:39a0d8604657ba9022aa5b88de3771f9a87f7a100187743f8b02c4995137f7c7`  
		Last Modified: Wed, 07 Sep 2022 21:20:09 GMT  
		Size: 1.2 MB (1215200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf75964ac643c8e0de2048260f7080c9a9afd12c87c3f93305892303c02626`  
		Last Modified: Wed, 07 Sep 2022 21:20:08 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:52932e74f09f4f600395ef0e65ac7761f74590c784de385b329c3deba73e9728
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122585761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceffdb3edb815118e8e62d2de89c304f5c9789a479a4aa646137643225c71277`
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
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:30 GMT
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
	-	`sha256:714c3b82fd5725d5c508bf921d8e44a826b6e80b7cf80206371441629020f7df`  
		Last Modified: Wed, 07 Sep 2022 20:50:44 GMT  
		Size: 1.2 MB (1162989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b035ad2bb7133b1e1f29d51c79911610b64ce645964402e0303856cc02a489d6`  
		Last Modified: Wed, 07 Sep 2022 20:50:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d54381d61daa9bbeb03bcbaa1c9fbf5e4890cd3f23fc2aebc13bb763bcd78efe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121421388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2fbb736245edf10b20547bdda39806040da01b5ed7daad738d04767e91fd47`
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
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:57:33 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:57:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:57:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:57:35 GMT
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
	-	`sha256:068f91f2941da883f37d54e440827226340fd3cad687e8529e236e235400c098`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 1.2 MB (1159978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae346762b582e00a5f229e741b110848ff0c3b95a30e95e56d235d7eed3c31`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e4ced291a901313117012e281dd0de28ec1d3c2e70246002d0533aea698925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121532298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3045db8e0202ea02304fde36f24f2fa1f10473c6b30d8dd9cc85392b3e63eab`
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
# Wed, 07 Sep 2022 20:39:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:39:42 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:39:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:39:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:39:46 GMT
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
	-	`sha256:5340d2088ba2060ab6fd7ac03124f5c7f395a51670305bf90a89da96988e8daa`  
		Last Modified: Wed, 07 Sep 2022 20:41:12 GMT  
		Size: 1.1 MB (1120446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5c4ba17c8241ba8dfbe915956db306ef689730489ef97462e99e641a0c1bf`  
		Last Modified: Wed, 07 Sep 2022 20:41:11 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:2cc10ae309cb5fac54e5e8d39dbef0f535d8ad5336c9b32415250274fcc0cfb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122072737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8c0fd8624128c41541d92222a799f89ca10620bd3b187579c1c6cba4827192`
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
# Wed, 07 Sep 2022 21:16:31 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:32 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:16:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:16:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:16:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:16:35 GMT
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
	-	`sha256:fdb755156f20625cf7436ebf9dd3e9d73ed62942073cbc911c4f42e739412d51`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 1.1 MB (1103854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be64bd7379e703449226d281d2a47bfacaf4193e886ff12bd078fa95dd5823f`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ef06f5dd643bb6af248afc42b5a46c88c13404a0b8718cf9ab9e5b07a36e6c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b9e4f098357534de1347fdb9b83e146abab58747e67d367d7e39f967d47b3a`
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
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:41:37 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:41:38 GMT
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
	-	`sha256:b6163d00c71b4379b800d1de8c81291389a7c79cc6d574dcce5e37183b3afde4`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 1.2 MB (1167442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532161760fe5ac59a0240e62f0bc251ea4e8de1f539811850f43e3802394e34`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fc7d6643b94f172dc0be1c2a55fe404556c0ef4308cd01485587e677fd69b58f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2.5.2-builder-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5bd4a15f1f1608bda512eef3fb6ab85a621321eaf331befc3460e95e84bbdfc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:7a5223f7720e5df685236b56c58dd57fad525b88fdb76e56e121a9e3be273615
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2494943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ea73be5cb10a5570dad83431d3aba123ed40e564b9f20fbf123f2be4546100`
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
# Wed, 07 Sep 2022 21:18:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:18:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:18:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:57 GMT
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
	-	`sha256:ff9d42bb565792710d4018b199ac636b9be0ffb9db23b35bc1eee69dca771c33`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61760b64ebc2bb823a7baca5dd0c0d7db3befbbed5ad1a8c1a5e6eaf346ca0b4`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f87d92375e5d9779ea8a646f053e96096f690a3c73617055f862f173f5033`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3271b3d777871daea415771bcf19be13bdf3d9fcd47e5c1777c9f480790716e`  
		Last Modified: Wed, 07 Sep 2022 21:27:15 GMT  
		Size: 1.9 MB (1868000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b438765ca79769b19f152009561021f6f8ac5c4446b1fc99e7fd9b10a4e8adba`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore`

```console
$ docker pull caddy@sha256:e93223c9604a42ed32a365ac8f0a2cb429b636c5cd64417763033237d281936d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8e736a0201648378f698716a66fc532320d11f8357cb58773c47b5cfe6cfed3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2.5.2-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e43f46a4015c9bdce6f65c400e02eca5ae6d1a642bfc498c1c231e8d60a8958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3`

```console
$ docker pull caddy@sha256:de23977011f7edd61599b12cd7ed1401ef840ddf5fef47ebac4644c57f933a3c
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

### `caddy:2.6.0-beta.3` - linux; amd64

```console
$ docker pull caddy@sha256:cb0afc7b8e9f273b4d092cf1967975f3908b348af603b62ca0c5acd8812b4b95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17551299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc25005c58f5a972b2532f5b1d93583894591ded8351ff10d88be40e8c5646`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 21:19:31 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:19:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 21:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 21:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 21:19:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 21:19:34 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:19:35 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:19:35 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:19:35 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:36 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:36 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:36 GMT
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
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ee5c4b6e2ab71e82a7e3fbf360a4b5ca82f328c63c1992890f26ee1b7ff377`  
		Last Modified: Wed, 07 Sep 2022 21:20:23 GMT  
		Size: 14.4 MB (14434750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39a6567e238aebbe4a6a9654fc6c4e60a2c8d933e036607059b6c8d5ab068c3`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - linux; arm variant v6

```console
$ docker pull caddy@sha256:68ba68ccbc3529943ee5f6dd4f502d4e6159e0ecf945140b4debe7a75d2dd259
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16757908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51c6bdee02ffc28c448699f17112046355d50d64f3a718310539b6bfd86fe1ca`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:49:39 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:49:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:49:43 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:49:43 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:49:44 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:49:44 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:49:45 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:45 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:45 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:45 GMT
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
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7a392f509c981e0e2cf1200d5bcf743a9cd13a0a6c60880df4edfc3adfc426`  
		Last Modified: Wed, 07 Sep 2022 20:51:01 GMT  
		Size: 13.8 MB (13833488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1070f182bd30a04e032100811c86c38683072e9c9bd2fa2d0d2f7a9b6ef86637`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0d13e7d01241baf7ddb221429be6198c52e0b8596647b011af00b99018c029e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16532812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c22ee1321c0f407a5e34b15da1cc9a091480858476971ec6e04872a40b10aa9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:57:47 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:57:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:57:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:57:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:57:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:57:51 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:53 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:53 GMT
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
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2589ae3c3ff75108e1cb9e92327022c66b0752e2b9b606607dd83882fdbebda7`  
		Last Modified: Wed, 07 Sep 2022 20:59:27 GMT  
		Size: 13.8 MB (13806152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f112754572fa5e49f98265da61bad6cfe772178b922b3020e7c6330ed268256`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3fb61df004c4dbb041ea4466395785efaba318ab5da9b539ccd0f3bf0a550b1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16172124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd25c09efb4ee688cf35eccd98723427d4d84c7068f76c9acf9096793a44bbc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:39:55 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:40:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:40:01 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:40:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:40:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:40:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:40:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:40:09 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:40:10 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:40:11 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:40:12 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:40:13 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:40:14 GMT
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
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102fb98ed9d8795d454181d901fdf889a4f7fd443954a990c88da7767c5d247`  
		Last Modified: Wed, 07 Sep 2022 20:41:27 GMT  
		Size: 13.2 MB (13154255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae76617de1b4e4cbd7e54d9e35d78135710c47a940aeee70821a49530e3356b`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - linux; ppc64le

```console
$ docker pull caddy@sha256:9b6e0d84a837f0027a33c5a7fdacbef6a87cd13e22e0c0660045ae3ea75f8b98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15934603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071d75a51e048037ba087ac1696414e77f1268a2bdd6ab401e53ba6a5538a257`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 21:16:44 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:16:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 21:16:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 21:16:49 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 21:16:50 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 21:16:50 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:16:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:16:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:16:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:16:52 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:16:53 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:16:53 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:53 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:53 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:54 GMT
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
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb99c363d6ec8b151ebc31cfd24ee0f95180e63bc2b84bd97196eaef74741d1d`  
		Last Modified: Wed, 07 Sep 2022 21:18:11 GMT  
		Size: 12.8 MB (12818791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e08992dd06133b5c8f38e0a7ac18ed93f4ef392a347c3536e032051acfb89`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - linux; s390x

```console
$ docker pull caddy@sha256:0043a6ac9029c984f730289f6ac97fea8ed4c3a0e6ac218662b18107754fd2ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16908165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2607b4c125dbc908d41176646382390bde28ee97ac3c07a62f54974fe5b33590`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:41:48 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:41:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:41:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:41:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:41:52 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:41:54 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:54 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:55 GMT
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
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e02a8a1a97a8a36c681b65c5d55bd7c0295751535c3e762e208706489ed9b9`  
		Last Modified: Wed, 07 Sep 2022 20:43:00 GMT  
		Size: 14.0 MB (14006844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97bdad04135f6e5331ca73b79792813b264ff143ff6e4c2e99f8a5ef3af37`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:88e9a60ea5b406bb189949479b4ae063a3cc4daf346989907c2685e65f555a8c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693256192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9797018ab22bc8f72282f5831dc6d9daf160a4b8b12adb24bce2e415c8ffa202`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:20:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 07 Sep 2022 21:20:07 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:21:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e1b60bb8faa2b88e40485b4a95dbd576e24907679b05de0c78362dec9fd5ed96d5ece4a141cf73a20909749b765832c51d2c5b31a59a77913d6db2ae40d3fd9e')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 07 Sep 2022 21:21:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 07 Sep 2022 21:21:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 07 Sep 2022 21:21:21 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:21:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:21:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:21:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:21:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:21:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:21:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:21:28 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:21:29 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:21:30 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:21:31 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:22:19 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:22:19 GMT
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
	-	`sha256:20a7620fe7390d1e63d1e62399c0e75ccb38893e7837c15ac7ba90408cc83f86`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 372.8 KB (372752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d876e92cdae5cc8ef8f030e1935cad493e3d813cb760e327fd3baede311dcfe`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463ae40d7b2aa49884fc8d8ed3005a6dd425600114d2e728dbfc614f584512aa`  
		Last Modified: Wed, 07 Sep 2022 21:27:38 GMT  
		Size: 14.8 MB (14838866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36767dc50f67b8b76415cb0e3e7e76c41358fba6d43a46a82b51c84f7fcca412`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30153786541aece4c50cd4feaf07ac1e53a36f4a8e6a8a630d76285b9653634`  
		Last Modified: Wed, 07 Sep 2022 21:27:33 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8507b8c34256d6baae79684ecc2b03d398caca3141f9da66f8026b30deb12085`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af74df38a1b632249cb4597afc4bffad364f4e30db87382262add3da672756`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d10ae4de6601a9309c0dba410a9cfbb82301be4d4a0f315d2b4c5f8a6210ca`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49cbbe83dc124d1b3f86656793dbfdba968f3900533b6b29da8b7343254a526`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab2e6b2e3f90f097c2155b5c40857c0d7c4283e1c0eafbb19f5fdea9db65cf`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa660547951fe9bc7670499947a22cbf88adb57999e85516eafef4f6ff659a12`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021b454c8d55b873abaee3ab57fe8cfb39d0118ee38ce18298d3769eb8dbe3f5`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67b8e44a69ddb26dfda0a5fda5de1089ab0dfb8df3048a7f1aa1899c477b39`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1e328f7bcf589db46bfe005176f9d34d5916ed38496fb02e91adb0aa302860`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c61328bb6e8a51d4176947cd19babf2660d872019ebb375fcac3c964f4d0bd`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04bcc5c65d2d12a1fbdeaf18184f5dee656aa0335ffbc70660fb526d5dc0c2`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3001db7818ba5ecfa3d8a02faf041ccb1c8a9035c947f48cd045d86e23724`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81cff48308bcf6bd0f2109bd09c0cb34f144b2dfba962ffbe1db73adaa08044`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 307.8 KB (307776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e8f8449020b921f999cd4b0b3e93e958938b8dbcfc9db331855ffea48129fa`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:279ca20d65d1a0dbf40b1604d3a452b33cb7ce2bc873b50ab7a5ff9349c5dcc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332992838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e7d089abaf2c47a1371b6cc08e96e8e2f8d24eec70f8e795c1b33e41c41c42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:22:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 07 Sep 2022 21:22:56 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:23:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e1b60bb8faa2b88e40485b4a95dbd576e24907679b05de0c78362dec9fd5ed96d5ece4a141cf73a20909749b765832c51d2c5b31a59a77913d6db2ae40d3fd9e')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 07 Sep 2022 21:23:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 07 Sep 2022 21:23:25 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 07 Sep 2022 21:23:25 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:23:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:23:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:23:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:23:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:23:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:23:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:23:33 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:23:34 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:23:35 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:23:35 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:23:51 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:23:51 GMT
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
	-	`sha256:e800f51c3128d9d98f99292311d8cfcf6aff80006f7a8610b980ead884f65a29`  
		Last Modified: Wed, 07 Sep 2022 21:27:52 GMT  
		Size: 643.9 KB (643929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9d35750bde1d736e80bee43c0544e38865aba250a2ac6b3c428e4497b5e9`  
		Last Modified: Wed, 07 Sep 2022 21:27:51 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e096b81de1a3f7284446be0432af41a5b4b58a5b456874bb7886de96b97045`  
		Last Modified: Wed, 07 Sep 2022 21:27:55 GMT  
		Size: 15.1 MB (15073702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8afff9325d899befdf790febe8d6142cd1e008afb2aff0fb176e1711c8e024`  
		Last Modified: Wed, 07 Sep 2022 21:27:51 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f35a82d111caffaec6bafc59ea718c162bc2ae84c7d634c033081c07972f9f3`  
		Last Modified: Wed, 07 Sep 2022 21:27:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1ec7808f718b2ac365a0c5af7d09c075a2d3f75020b3d3db706ac4425edfaf`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ebcd9bfe65cef6c4975d67ebf7b37c35b48b5046eb4e5581e77c354b9349b`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de39d1b5849b53cc129cd72b574ce78b52ca0dba835ab46a98a166ccdb2e02fd`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf11f1b9544e317d2e09673b919829f493568d4ffb8236b7c2105bda0f52169`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c698e9f047b2d855747c32d2e660afc04a04c9570624fd7f792fe060b0f08c61`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d44eaacad0442a25d182c0faf18fcefc6b0c02b327561dd3d2df32401a4b0c6`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c186860413e353a19dfb7f22b1d48869e7e720c7ab0508da3f105093e6fe9975`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268b1ccdf4a335813076c750d368ab8f04db9534b2b5e454c494ee776db1170d`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b02eaa6ac31096cc6562add0004b5fe5fa82e59219a3ee730adf10cec446ce`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff70701765ddae8ec2dc248ceaf0c3c97120f51a735849f66862a5eb86cb716`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4625089d3ed10e20d572f2eddd8bf4169910d1ed63d57c4030be559b05da75`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf421c38a1a3e7743511ebabb7d28c7319fd0965e26754e37cea36165c40140`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f32c77ce0b1df0939a5f81dcbf90048c1e73dc9c95104b3fb56e8e6f5783ef`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 362.0 KB (362019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e4a21c72bbb60e33f61928df738e312a1dd374ad361df032542d4fa0c77c6`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-alpine`

```console
$ docker pull caddy@sha256:de7cf7148e99504767a9cfa230f2b45a6aa0d715bbc730d6cd796f6439782fe2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.0-beta.3-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:cb0afc7b8e9f273b4d092cf1967975f3908b348af603b62ca0c5acd8812b4b95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17551299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70dc25005c58f5a972b2532f5b1d93583894591ded8351ff10d88be40e8c5646`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 21:19:31 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:19:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 21:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 21:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 21:19:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 21:19:34 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:19:35 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:19:35 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:19:35 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:36 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:36 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:36 GMT
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
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ee5c4b6e2ab71e82a7e3fbf360a4b5ca82f328c63c1992890f26ee1b7ff377`  
		Last Modified: Wed, 07 Sep 2022 21:20:23 GMT  
		Size: 14.4 MB (14434750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39a6567e238aebbe4a6a9654fc6c4e60a2c8d933e036607059b6c8d5ab068c3`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:68ba68ccbc3529943ee5f6dd4f502d4e6159e0ecf945140b4debe7a75d2dd259
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16757908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51c6bdee02ffc28c448699f17112046355d50d64f3a718310539b6bfd86fe1ca`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:49:39 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:49:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:49:43 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:49:43 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:49:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:49:44 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:49:44 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:49:45 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:45 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:45 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:45 GMT
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
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7a392f509c981e0e2cf1200d5bcf743a9cd13a0a6c60880df4edfc3adfc426`  
		Last Modified: Wed, 07 Sep 2022 20:51:01 GMT  
		Size: 13.8 MB (13833488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1070f182bd30a04e032100811c86c38683072e9c9bd2fa2d0d2f7a9b6ef86637`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0d13e7d01241baf7ddb221429be6198c52e0b8596647b011af00b99018c029e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16532812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c22ee1321c0f407a5e34b15da1cc9a091480858476971ec6e04872a40b10aa9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:57:47 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:57:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:57:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:57:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:57:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:57:51 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:57:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:53 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:53 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:53 GMT
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
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2589ae3c3ff75108e1cb9e92327022c66b0752e2b9b606607dd83882fdbebda7`  
		Last Modified: Wed, 07 Sep 2022 20:59:27 GMT  
		Size: 13.8 MB (13806152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f112754572fa5e49f98265da61bad6cfe772178b922b3020e7c6330ed268256`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3fb61df004c4dbb041ea4466395785efaba318ab5da9b539ccd0f3bf0a550b1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16172124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd25c09efb4ee688cf35eccd98723427d4d84c7068f76c9acf9096793a44bbc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:39:55 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:40:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:40:01 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:40:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:40:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:40:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:40:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:40:09 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:40:10 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:40:11 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:40:12 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:40:13 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:40:14 GMT
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
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102fb98ed9d8795d454181d901fdf889a4f7fd443954a990c88da7767c5d247`  
		Last Modified: Wed, 07 Sep 2022 20:41:27 GMT  
		Size: 13.2 MB (13154255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae76617de1b4e4cbd7e54d9e35d78135710c47a940aeee70821a49530e3356b`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9b6e0d84a837f0027a33c5a7fdacbef6a87cd13e22e0c0660045ae3ea75f8b98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15934603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071d75a51e048037ba087ac1696414e77f1268a2bdd6ab401e53ba6a5538a257`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 21:16:44 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:16:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 21:16:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 21:16:49 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 21:16:50 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 21:16:50 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:16:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:16:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:16:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:16:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:16:52 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:16:53 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:16:53 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:53 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:53 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:54 GMT
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
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb99c363d6ec8b151ebc31cfd24ee0f95180e63bc2b84bd97196eaef74741d1d`  
		Last Modified: Wed, 07 Sep 2022 21:18:11 GMT  
		Size: 12.8 MB (12818791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e08992dd06133b5c8f38e0a7ac18ed93f4ef392a347c3536e032051acfb89`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0043a6ac9029c984f730289f6ac97fea8ed4c3a0e6ac218662b18107754fd2ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16908165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2607b4c125dbc908d41176646382390bde28ee97ac3c07a62f54974fe5b33590`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 07 Sep 2022 20:41:48 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:41:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4fd35ccbf42ace902e1fa196b7cb52bfbd9eb49907b10e46a256072516336a78de23b0bbd548efc8254693b73862ee1705aeb1696cacfc6452f8faed62d60e65' ;; 		armhf)   binArch='armv6'; checksum='357f1053c87327631c8f8b66e19b662a9feb3d3cd85346ca726ac64b4cb6005781b7af4c1c23eadfd8a6099d3dc50eb375e8caf3227072f24f42ac1e15647d5e' ;; 		armv7)   binArch='armv7'; checksum='26fe73813a6897424d4d2c584644c3bd96e6e57a63b3d4643edb3bd33f75bb6e8de8f6c5378c00dd19f562e54966afe55bcf58a2ba77ac5aa4c58b6006a65a51' ;; 		aarch64) binArch='arm64'; checksum='0637a726186c6ff15988e1a528a5b680b60d23c016e68e7f52224b556d92825e228bf9fa4e4d0be48ce23344a7b186016f9119a6fb4686747c525c80837713eb' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='8b2c8d8e5f80dc441bb1189966be70510bfd6147867e0a8e61c5afb5be85e054f7e7e453894fa0f7fd33f18d73ee1f85b175d548e7c09e9733d096b5c3281ed7' ;; 		s390x)   binArch='s390x'; checksum='fbaf777d888e96ce7061c5f8e3fa399086ba3dcf1656d2ab365ee275857f9853d9586ca3f90698b8bf3a2dc098891266db0301d2d6f15dba036a288d035e3ac2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 07 Sep 2022 20:41:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 07 Sep 2022 20:41:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 07 Sep 2022 20:41:52 GMT
ENV XDG_DATA_HOME=/data
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 20:41:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 20:41:54 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 80
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 443
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:54 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:54 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:55 GMT
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
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e02a8a1a97a8a36c681b65c5d55bd7c0295751535c3e762e208706489ed9b9`  
		Last Modified: Wed, 07 Sep 2022 20:43:00 GMT  
		Size: 14.0 MB (14006844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97bdad04135f6e5331ca73b79792813b264ff143ff6e4c2e99f8a5ef3af37`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-builder`

```console
$ docker pull caddy@sha256:0b40db4443db690143a32b8146c6946e026a412aa2eea31cc08d1d1ece144150
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

### `caddy:2.6.0-beta.3-builder` - linux; amd64

```console
$ docker pull caddy@sha256:673e8a9430311fd1f1c6be46c37368f172d8d8fd1c3d8735f9bd2f3343302332
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133472237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf703f000c2701fc63eff705ba3946d0ad6206d110cc0aecb4eea2ec9d2e6be`
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
# Tue, 06 Sep 2022 19:20:35 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:22:15 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:22:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:22:16 GMT
WORKDIR /go
# Wed, 07 Sep 2022 21:19:39 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:40 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:41 GMT
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
	-	`sha256:6569e6eb40cde4a09139a057e6c7dbf5374570c71414b4d2a0b5d0a1c8a13368`  
		Last Modified: Tue, 06 Sep 2022 19:30:47 GMT  
		Size: 122.2 MB (122223942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601c7710d0ea88e955c805e670079857228eee7e515b89e4e953e05a6f80d2ad`  
		Last Modified: Tue, 06 Sep 2022 19:30:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c472cbc8629c6e976646511fb3733e0c47037cd0b7505baa1da11468dcbe65c8`  
		Last Modified: Wed, 07 Sep 2022 21:20:31 GMT  
		Size: 6.9 MB (6941616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c252f1cbf518869bf72c0356add4f0c08cdaf60ca9fa25e07ce182c57e76aeb0`  
		Last Modified: Wed, 07 Sep 2022 21:20:30 GMT  
		Size: 1.2 MB (1215185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3dbd7752eb27b97a7eb2e6b204345c30be85faf18108bdee8ddde2220abaea`  
		Last Modified: Wed, 07 Sep 2022 21:20:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3fec6c5831238296b5c85ee5e1bbed51fdb6ac53c710f992a09b849613b1537a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129472980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88e0ebce6fd2abc4ac26ea1c82b210ad3894344e9ce2bf20ba7b589eaf9615c2`
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
# Tue, 06 Sep 2022 18:49:22 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 18:55:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 18:55:43 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 18:55:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 18:55:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 18:55:43 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:49:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:49:51 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:51 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:49:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:53 GMT
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
	-	`sha256:b37f5a0ac6468f4b4626529f5ac53a55230a713f6c134942e6ab8159e6b0b8b0`  
		Last Modified: Tue, 06 Sep 2022 19:18:20 GMT  
		Size: 118.6 MB (118602506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9ef52c98a8db81bd037b179d32843186f7628971342eaf00a000c9aea43d33`  
		Last Modified: Tue, 06 Sep 2022 19:17:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21968742fd47ffacdf24a121cfba8df304e9d4ad64981b1a40819a5feb77ce7d`  
		Last Modified: Wed, 07 Sep 2022 20:51:10 GMT  
		Size: 6.8 MB (6808137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5237fbaff7dcc6fd8d7839fe9a2b93d5adf48c601706e478e9526a38b0f0d73d`  
		Last Modified: Wed, 07 Sep 2022 20:51:09 GMT  
		Size: 1.2 MB (1162981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e014ea3e1c1063d5383d1257cb04894097bcf7e029364cbbd27e412fe58c9e`  
		Last Modified: Wed, 07 Sep 2022 20:51:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4da3e93a9a7aa8b28dfc8098daf8d9b02f299a349df84a313a404b08f4b53f8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128285841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3934048437c84c3129639437177a845a51c1c7479f26de9b04c5a91a02730173`
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
# Tue, 06 Sep 2022 18:59:19 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:07:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:07:05 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:07:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:07:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:07:06 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:58:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:58:02 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:58:02 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:58:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:58:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:58:04 GMT
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
	-	`sha256:94b896143eb263ebd8ed2b1ad916b629a238d21ec33d71258121537afe2e2844`  
		Last Modified: Tue, 06 Sep 2022 19:26:53 GMT  
		Size: 118.4 MB (118356471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7b8b34ca0558d990f998e44190eda4151a594a4f72478a4979b0de641f4341`  
		Last Modified: Tue, 06 Sep 2022 19:26:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f20f5019b3f3995b2f3c129ff7d87cf7ca12dc27c101b68fad64a94ddb7b38`  
		Last Modified: Wed, 07 Sep 2022 20:59:37 GMT  
		Size: 6.1 MB (6067800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9981bf2d10d35713b49e63872e484e81187a604e4a66b2c813c0fb14eac133`  
		Last Modified: Wed, 07 Sep 2022 20:59:36 GMT  
		Size: 1.2 MB (1159975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a565c5f3da483401e396ab2c99cd0bdfef542d47bc8ed26f5d08eefcfa1e90`  
		Last Modified: Wed, 07 Sep 2022 20:59:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4e0f2e8fbfd2b45d8d98d10086a070f734e5f89d7e1d3cb6d96842819623217c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127966957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194408722253039fc2523511a38a24ef5e55f83671253dcc3bc7879fe28811a3`
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
# Tue, 06 Sep 2022 19:57:56 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:59:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:59:35 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:59:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:59:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:59:37 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:40:21 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:40:22 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:40:22 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:40:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:40:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:40:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:40:26 GMT
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
	-	`sha256:2e5ac390c5545179ffc399eeb0dc80bd8a348a1c8c0cabaf80a59e427c4ac37b`  
		Last Modified: Tue, 06 Sep 2022 20:08:11 GMT  
		Size: 116.8 MB (116801390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5539c8b2b31eb6679625c9cb51df982d12b432fce3030efb19cbd8e2317e4d92`  
		Last Modified: Tue, 06 Sep 2022 20:07:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b14d485599ae2fb014a923e42fc8a503a9538b595e809701a3f6f8627096e`  
		Last Modified: Wed, 07 Sep 2022 20:41:36 GMT  
		Size: 7.1 MB (7052251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e93b382c41df2150b4d98d098dd69b43460ec50e289e1da348d4a909a8477c`  
		Last Modified: Wed, 07 Sep 2022 20:41:35 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cecbc796de06842c105507f7173b0827c35ed2e94e97c6d9d0df4630ec7e7`  
		Last Modified: Wed, 07 Sep 2022 20:41:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:d12de885ffaa83552e2619adb83e2f7939f3303aec635093b7b95ec03323f365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128847060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5791b2d98e772843d096d5642188706fafa9446ccf3bd5fcb84a1a8c260e26`
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
# Tue, 06 Sep 2022 19:17:21 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:20:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:20:15 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:20:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:20:16 GMT
WORKDIR /go
# Wed, 07 Sep 2022 21:17:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 21:17:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:17:01 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:17:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:17:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:17:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:17:04 GMT
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
	-	`sha256:6524907b27c0539743e58589742ab7661e17d66be3c41d6acff03ba9564c292b`  
		Last Modified: Tue, 06 Sep 2022 19:32:16 GMT  
		Size: 117.2 MB (117170200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daea48cd0f015b1ef6f5b4c3f24e12460ff1ffead8f5d48b5c64f2f304fe43ce`  
		Last Modified: Tue, 06 Sep 2022 19:31:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7736e417f8158a33c99ce39d954a0ec249ae3905af116366a002cb74d23a8b59`  
		Last Modified: Wed, 07 Sep 2022 21:18:21 GMT  
		Size: 7.5 MB (7482243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617dfbdf3fdaa77c563adcf722043ff564327e5f5a9935ae055b8fb2d4e2ce4d`  
		Last Modified: Wed, 07 Sep 2022 21:18:19 GMT  
		Size: 1.1 MB (1103848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47e072798c5015f69bf7c904b16d599e72331046a9ccec1176854a6edfc013b`  
		Last Modified: Wed, 07 Sep 2022 21:18:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - linux; s390x

```console
$ docker pull caddy@sha256:e44fc41871f7e3d41f8b2ff92a49e53bbbfb7bb38c74060bdac2b1561954054e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131795470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a68568325a534f0529659d84b215020db43975b16a19984c898d21df17917e5`
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
# Tue, 06 Sep 2022 19:48:50 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:50:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:50:46 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:50:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:50:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:50:47 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:42:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:42:03 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:42:03 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:42:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:42:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:42:04 GMT
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
	-	`sha256:96dd28a57d468c751b390aa771cc0c96a8da30086f6465c57db35b2d764fdd04`  
		Last Modified: Tue, 06 Sep 2022 19:58:52 GMT  
		Size: 120.7 MB (120698828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80248e4ad120c36e15983455faa1dd0659d7f6fa484fb6da33c3a2a5014eade6`  
		Last Modified: Tue, 06 Sep 2022 19:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0534a6362c2a5a3390e4055fe4dc0a6b85c67cd228925ae6ab84508630d02d`  
		Last Modified: Wed, 07 Sep 2022 20:43:05 GMT  
		Size: 7.1 MB (7052949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a691799fb1b17dc8f6d44487cb06a74215786cc473e4d6d4976c4d4b6154ae1`  
		Last Modified: Wed, 07 Sep 2022 20:43:04 GMT  
		Size: 1.2 MB (1167436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d4decb5bc33616850bfc2248fae17e1dd8fd41c68049335a2b12e253ab7162`  
		Last Modified: Wed, 07 Sep 2022 20:43:04 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3a1df5d8540fe04700054e76364921460769165b9e358f200c73dc19dfefd4fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2862712804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5ffa7f2ebc62a4fb7fbed77c359b54f580947db647dade703c18a1b95739d0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:19:35 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:23:55 GMT
RUN $url = 'https://dl.google.com/go/go1.19.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b33584c1d93b0e9c783de876b7aa99d3018bdeccd396aeb6d516a74e9d88d55f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:23:57 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:24:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:24:02 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:24:03 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:24:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:25:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:25:07 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326b771a7d97ee74903352b5566ccb2d5603e0a5befa73f593ab5e90148e176`  
		Last Modified: Tue, 06 Sep 2022 19:49:29 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd7fefccc0ffce5c9671b318e7aa208c629aef78fd3de7d62c31e1f7c5d1270`  
		Last Modified: Tue, 06 Sep 2022 19:50:05 GMT  
		Size: 157.6 MB (157595150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea8b66b68cf72f87532ca5529bcc4d986ed4545e9e409893911202c37cef905`  
		Last Modified: Tue, 06 Sep 2022 19:49:29 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bde95c643b821c1831f1288448405ca778ac8b5d16367fe28059ae5d1d8e1`  
		Last Modified: Wed, 07 Sep 2022 21:28:04 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0340e75d6568477a12dcfa822a8c94319749f23edd9b222a3845a81a6b59ff`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ae305451894c846605df1544c201caccdb64f2b41971fdb28d2c2545f21d1`  
		Last Modified: Wed, 07 Sep 2022 21:28:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28ca3f99d06459eef007f08d25bbdabacf47e022c7b80b7795ddfd11057ec44`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122e2dbea68b89bd80fc84fad9c94323a7dde9da3491878e1c4bd42545b77525`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.6 MB (1629839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea041a15aeb797c02f0e6076b9acd7474452cdeed4ed3838efbe256cdcff932`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:3418320d08bca08fe61d600099eb612cdbb009eb5cd3a0d7aeeb28bc9ec1a207
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2502851272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b119bfd6d744bc5ed3a8b2726c825a646f3d0b2c0b4bc85e647605a5175091e`
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
# Tue, 06 Sep 2022 19:16:07 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:19:13 GMT
RUN $url = 'https://dl.google.com/go/go1.19.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b33584c1d93b0e9c783de876b7aa99d3018bdeccd396aeb6d516a74e9d88d55f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:19:15 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:25:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:25:15 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:25:16 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:25:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:25:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:25:42 GMT
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
	-	`sha256:d5f9102f80120b26e1ec1595d0a52709fc6daee1dbded5cc466d75350e67441a`  
		Last Modified: Tue, 06 Sep 2022 19:48:35 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53861b53c0dcf69aa2f04aa09ec5df3e405846fbeb8f4ecf89c5208cc1aa28b`  
		Last Modified: Tue, 06 Sep 2022 19:49:14 GMT  
		Size: 157.8 MB (157803876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b467314e5cf39039a1455d655c11778d821fcf8a96524389e050f0a728cbc7`  
		Last Modified: Tue, 06 Sep 2022 19:48:35 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd5d68ce2942424d62ce9e4224839cedc42c4baf596293576562a7c3166aa8`  
		Last Modified: Wed, 07 Sep 2022 21:28:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd00ac54a789a066e8399aa678152986191a175376a7852a8bf20001b09207f`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b18b660e0f785051b7744bb756d353e5c25f8cc6ddd523bc9a38157f32ca134`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b68c4a26e71335f56ecda1992b04fa03eced242475eda294b58fb75c40714e`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564afc1032e0ccc966cdf34b2937623f2eb1a05a9885d44fd42ee5b66b465d0`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.9 MB (1867709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539c1b076857f4819a445a7948cf2ddf8c7f4a2f3c80a71f112b8ddb23f82fea`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-builder-alpine`

```console
$ docker pull caddy@sha256:53958aedab93e0877fabcdbfbf783aa0b2aaeda1d32b52d8ade7bd283d061b8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.0-beta.3-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:673e8a9430311fd1f1c6be46c37368f172d8d8fd1c3d8735f9bd2f3343302332
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133472237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf703f000c2701fc63eff705ba3946d0ad6206d110cc0aecb4eea2ec9d2e6be`
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
# Tue, 06 Sep 2022 19:20:35 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:22:15 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:22:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:22:16 GMT
WORKDIR /go
# Wed, 07 Sep 2022 21:19:39 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:40 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:41 GMT
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
	-	`sha256:6569e6eb40cde4a09139a057e6c7dbf5374570c71414b4d2a0b5d0a1c8a13368`  
		Last Modified: Tue, 06 Sep 2022 19:30:47 GMT  
		Size: 122.2 MB (122223942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601c7710d0ea88e955c805e670079857228eee7e515b89e4e953e05a6f80d2ad`  
		Last Modified: Tue, 06 Sep 2022 19:30:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c472cbc8629c6e976646511fb3733e0c47037cd0b7505baa1da11468dcbe65c8`  
		Last Modified: Wed, 07 Sep 2022 21:20:31 GMT  
		Size: 6.9 MB (6941616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c252f1cbf518869bf72c0356add4f0c08cdaf60ca9fa25e07ce182c57e76aeb0`  
		Last Modified: Wed, 07 Sep 2022 21:20:30 GMT  
		Size: 1.2 MB (1215185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3dbd7752eb27b97a7eb2e6b204345c30be85faf18108bdee8ddde2220abaea`  
		Last Modified: Wed, 07 Sep 2022 21:20:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3fec6c5831238296b5c85ee5e1bbed51fdb6ac53c710f992a09b849613b1537a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129472980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88e0ebce6fd2abc4ac26ea1c82b210ad3894344e9ce2bf20ba7b589eaf9615c2`
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
# Tue, 06 Sep 2022 18:49:22 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 18:55:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 18:55:43 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 18:55:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 18:55:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 18:55:43 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:49:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:49:51 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:51 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:49:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:53 GMT
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
	-	`sha256:b37f5a0ac6468f4b4626529f5ac53a55230a713f6c134942e6ab8159e6b0b8b0`  
		Last Modified: Tue, 06 Sep 2022 19:18:20 GMT  
		Size: 118.6 MB (118602506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9ef52c98a8db81bd037b179d32843186f7628971342eaf00a000c9aea43d33`  
		Last Modified: Tue, 06 Sep 2022 19:17:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21968742fd47ffacdf24a121cfba8df304e9d4ad64981b1a40819a5feb77ce7d`  
		Last Modified: Wed, 07 Sep 2022 20:51:10 GMT  
		Size: 6.8 MB (6808137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5237fbaff7dcc6fd8d7839fe9a2b93d5adf48c601706e478e9526a38b0f0d73d`  
		Last Modified: Wed, 07 Sep 2022 20:51:09 GMT  
		Size: 1.2 MB (1162981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e014ea3e1c1063d5383d1257cb04894097bcf7e029364cbbd27e412fe58c9e`  
		Last Modified: Wed, 07 Sep 2022 20:51:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4da3e93a9a7aa8b28dfc8098daf8d9b02f299a349df84a313a404b08f4b53f8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128285841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3934048437c84c3129639437177a845a51c1c7479f26de9b04c5a91a02730173`
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
# Tue, 06 Sep 2022 18:59:19 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:07:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:07:05 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:07:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:07:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:07:06 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:58:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:58:02 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:58:02 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:58:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:58:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:58:04 GMT
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
	-	`sha256:94b896143eb263ebd8ed2b1ad916b629a238d21ec33d71258121537afe2e2844`  
		Last Modified: Tue, 06 Sep 2022 19:26:53 GMT  
		Size: 118.4 MB (118356471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7b8b34ca0558d990f998e44190eda4151a594a4f72478a4979b0de641f4341`  
		Last Modified: Tue, 06 Sep 2022 19:26:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f20f5019b3f3995b2f3c129ff7d87cf7ca12dc27c101b68fad64a94ddb7b38`  
		Last Modified: Wed, 07 Sep 2022 20:59:37 GMT  
		Size: 6.1 MB (6067800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9981bf2d10d35713b49e63872e484e81187a604e4a66b2c813c0fb14eac133`  
		Last Modified: Wed, 07 Sep 2022 20:59:36 GMT  
		Size: 1.2 MB (1159975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a565c5f3da483401e396ab2c99cd0bdfef542d47bc8ed26f5d08eefcfa1e90`  
		Last Modified: Wed, 07 Sep 2022 20:59:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4e0f2e8fbfd2b45d8d98d10086a070f734e5f89d7e1d3cb6d96842819623217c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127966957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194408722253039fc2523511a38a24ef5e55f83671253dcc3bc7879fe28811a3`
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
# Tue, 06 Sep 2022 19:57:56 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:59:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:59:35 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:59:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:59:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:59:37 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:40:21 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:40:22 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:40:22 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:40:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:40:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:40:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:40:26 GMT
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
	-	`sha256:2e5ac390c5545179ffc399eeb0dc80bd8a348a1c8c0cabaf80a59e427c4ac37b`  
		Last Modified: Tue, 06 Sep 2022 20:08:11 GMT  
		Size: 116.8 MB (116801390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5539c8b2b31eb6679625c9cb51df982d12b432fce3030efb19cbd8e2317e4d92`  
		Last Modified: Tue, 06 Sep 2022 20:07:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b14d485599ae2fb014a923e42fc8a503a9538b595e809701a3f6f8627096e`  
		Last Modified: Wed, 07 Sep 2022 20:41:36 GMT  
		Size: 7.1 MB (7052251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e93b382c41df2150b4d98d098dd69b43460ec50e289e1da348d4a909a8477c`  
		Last Modified: Wed, 07 Sep 2022 20:41:35 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cecbc796de06842c105507f7173b0827c35ed2e94e97c6d9d0df4630ec7e7`  
		Last Modified: Wed, 07 Sep 2022 20:41:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d12de885ffaa83552e2619adb83e2f7939f3303aec635093b7b95ec03323f365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128847060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5791b2d98e772843d096d5642188706fafa9446ccf3bd5fcb84a1a8c260e26`
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
# Tue, 06 Sep 2022 19:17:21 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:20:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:20:15 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:20:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:20:16 GMT
WORKDIR /go
# Wed, 07 Sep 2022 21:17:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 21:17:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:17:01 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:17:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:17:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:17:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:17:04 GMT
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
	-	`sha256:6524907b27c0539743e58589742ab7661e17d66be3c41d6acff03ba9564c292b`  
		Last Modified: Tue, 06 Sep 2022 19:32:16 GMT  
		Size: 117.2 MB (117170200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daea48cd0f015b1ef6f5b4c3f24e12460ff1ffead8f5d48b5c64f2f304fe43ce`  
		Last Modified: Tue, 06 Sep 2022 19:31:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7736e417f8158a33c99ce39d954a0ec249ae3905af116366a002cb74d23a8b59`  
		Last Modified: Wed, 07 Sep 2022 21:18:21 GMT  
		Size: 7.5 MB (7482243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617dfbdf3fdaa77c563adcf722043ff564327e5f5a9935ae055b8fb2d4e2ce4d`  
		Last Modified: Wed, 07 Sep 2022 21:18:19 GMT  
		Size: 1.1 MB (1103848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47e072798c5015f69bf7c904b16d599e72331046a9ccec1176854a6edfc013b`  
		Last Modified: Wed, 07 Sep 2022 21:18:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e44fc41871f7e3d41f8b2ff92a49e53bbbfb7bb38c74060bdac2b1561954054e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131795470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a68568325a534f0529659d84b215020db43975b16a19984c898d21df17917e5`
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
# Tue, 06 Sep 2022 19:48:50 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:50:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:50:46 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:50:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:50:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:50:47 GMT
WORKDIR /go
# Wed, 07 Sep 2022 20:42:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 07 Sep 2022 20:42:03 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:42:03 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 20:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:42:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:42:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:42:04 GMT
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
	-	`sha256:96dd28a57d468c751b390aa771cc0c96a8da30086f6465c57db35b2d764fdd04`  
		Last Modified: Tue, 06 Sep 2022 19:58:52 GMT  
		Size: 120.7 MB (120698828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80248e4ad120c36e15983455faa1dd0659d7f6fa484fb6da33c3a2a5014eade6`  
		Last Modified: Tue, 06 Sep 2022 19:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0534a6362c2a5a3390e4055fe4dc0a6b85c67cd228925ae6ab84508630d02d`  
		Last Modified: Wed, 07 Sep 2022 20:43:05 GMT  
		Size: 7.1 MB (7052949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a691799fb1b17dc8f6d44487cb06a74215786cc473e4d6d4976c4d4b6154ae1`  
		Last Modified: Wed, 07 Sep 2022 20:43:04 GMT  
		Size: 1.2 MB (1167436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d4decb5bc33616850bfc2248fae17e1dd8fd41c68049335a2b12e253ab7162`  
		Last Modified: Wed, 07 Sep 2022 20:43:04 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4db934f7ba52c567ebcd47b0ec61df101e10ee1af64f3a3fdebb9eab884bd5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2.6.0-beta.3-builder-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3a1df5d8540fe04700054e76364921460769165b9e358f200c73dc19dfefd4fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2862712804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5ffa7f2ebc62a4fb7fbed77c359b54f580947db647dade703c18a1b95739d0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:19:35 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:23:55 GMT
RUN $url = 'https://dl.google.com/go/go1.19.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b33584c1d93b0e9c783de876b7aa99d3018bdeccd396aeb6d516a74e9d88d55f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:23:57 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:24:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:24:02 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:24:03 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:24:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:25:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:25:07 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326b771a7d97ee74903352b5566ccb2d5603e0a5befa73f593ab5e90148e176`  
		Last Modified: Tue, 06 Sep 2022 19:49:29 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd7fefccc0ffce5c9671b318e7aa208c629aef78fd3de7d62c31e1f7c5d1270`  
		Last Modified: Tue, 06 Sep 2022 19:50:05 GMT  
		Size: 157.6 MB (157595150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea8b66b68cf72f87532ca5529bcc4d986ed4545e9e409893911202c37cef905`  
		Last Modified: Tue, 06 Sep 2022 19:49:29 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bde95c643b821c1831f1288448405ca778ac8b5d16367fe28059ae5d1d8e1`  
		Last Modified: Wed, 07 Sep 2022 21:28:04 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0340e75d6568477a12dcfa822a8c94319749f23edd9b222a3845a81a6b59ff`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588ae305451894c846605df1544c201caccdb64f2b41971fdb28d2c2545f21d1`  
		Last Modified: Wed, 07 Sep 2022 21:28:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28ca3f99d06459eef007f08d25bbdabacf47e022c7b80b7795ddfd11057ec44`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122e2dbea68b89bd80fc84fad9c94323a7dde9da3491878e1c4bd42545b77525`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.6 MB (1629839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea041a15aeb797c02f0e6076b9acd7474452cdeed4ed3838efbe256cdcff932`  
		Last Modified: Wed, 07 Sep 2022 21:28:02 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:efce3a410c5d84931f38795f23c5b3ccfc27fbda5c25d86302306787fa8ae7cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2.6.0-beta.3-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:3418320d08bca08fe61d600099eb612cdbb009eb5cd3a0d7aeeb28bc9ec1a207
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2502851272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b119bfd6d744bc5ed3a8b2726c825a646f3d0b2c0b4bc85e647605a5175091e`
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
# Tue, 06 Sep 2022 19:16:07 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:19:13 GMT
RUN $url = 'https://dl.google.com/go/go1.19.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b33584c1d93b0e9c783de876b7aa99d3018bdeccd396aeb6d516a74e9d88d55f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:19:15 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:25:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:25:15 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:25:16 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:25:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:25:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:25:42 GMT
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
	-	`sha256:d5f9102f80120b26e1ec1595d0a52709fc6daee1dbded5cc466d75350e67441a`  
		Last Modified: Tue, 06 Sep 2022 19:48:35 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53861b53c0dcf69aa2f04aa09ec5df3e405846fbeb8f4ecf89c5208cc1aa28b`  
		Last Modified: Tue, 06 Sep 2022 19:49:14 GMT  
		Size: 157.8 MB (157803876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b467314e5cf39039a1455d655c11778d821fcf8a96524389e050f0a728cbc7`  
		Last Modified: Tue, 06 Sep 2022 19:48:35 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd5d68ce2942424d62ce9e4224839cedc42c4baf596293576562a7c3166aa8`  
		Last Modified: Wed, 07 Sep 2022 21:28:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd00ac54a789a066e8399aa678152986191a175376a7852a8bf20001b09207f`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b18b660e0f785051b7744bb756d353e5c25f8cc6ddd523bc9a38157f32ca134`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b68c4a26e71335f56ecda1992b04fa03eced242475eda294b58fb75c40714e`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564afc1032e0ccc966cdf34b2937623f2eb1a05a9885d44fd42ee5b66b465d0`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.9 MB (1867709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539c1b076857f4819a445a7948cf2ddf8c7f4a2f3c80a71f112b8ddb23f82fea`  
		Last Modified: Wed, 07 Sep 2022 21:28:11 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-windowsservercore`

```console
$ docker pull caddy@sha256:4edf5a63e96842bb545ffb0c8175da9bc306731218e3043be057995f7172e5c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2.6.0-beta.3-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:88e9a60ea5b406bb189949479b4ae063a3cc4daf346989907c2685e65f555a8c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693256192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9797018ab22bc8f72282f5831dc6d9daf160a4b8b12adb24bce2e415c8ffa202`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:20:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 07 Sep 2022 21:20:07 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:21:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e1b60bb8faa2b88e40485b4a95dbd576e24907679b05de0c78362dec9fd5ed96d5ece4a141cf73a20909749b765832c51d2c5b31a59a77913d6db2ae40d3fd9e')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 07 Sep 2022 21:21:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 07 Sep 2022 21:21:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 07 Sep 2022 21:21:21 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:21:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:21:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:21:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:21:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:21:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:21:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:21:28 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:21:29 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:21:30 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:21:31 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:22:19 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:22:19 GMT
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
	-	`sha256:20a7620fe7390d1e63d1e62399c0e75ccb38893e7837c15ac7ba90408cc83f86`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 372.8 KB (372752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d876e92cdae5cc8ef8f030e1935cad493e3d813cb760e327fd3baede311dcfe`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463ae40d7b2aa49884fc8d8ed3005a6dd425600114d2e728dbfc614f584512aa`  
		Last Modified: Wed, 07 Sep 2022 21:27:38 GMT  
		Size: 14.8 MB (14838866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36767dc50f67b8b76415cb0e3e7e76c41358fba6d43a46a82b51c84f7fcca412`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30153786541aece4c50cd4feaf07ac1e53a36f4a8e6a8a630d76285b9653634`  
		Last Modified: Wed, 07 Sep 2022 21:27:33 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8507b8c34256d6baae79684ecc2b03d398caca3141f9da66f8026b30deb12085`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af74df38a1b632249cb4597afc4bffad364f4e30db87382262add3da672756`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d10ae4de6601a9309c0dba410a9cfbb82301be4d4a0f315d2b4c5f8a6210ca`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49cbbe83dc124d1b3f86656793dbfdba968f3900533b6b29da8b7343254a526`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab2e6b2e3f90f097c2155b5c40857c0d7c4283e1c0eafbb19f5fdea9db65cf`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa660547951fe9bc7670499947a22cbf88adb57999e85516eafef4f6ff659a12`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021b454c8d55b873abaee3ab57fe8cfb39d0118ee38ce18298d3769eb8dbe3f5`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67b8e44a69ddb26dfda0a5fda5de1089ab0dfb8df3048a7f1aa1899c477b39`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1e328f7bcf589db46bfe005176f9d34d5916ed38496fb02e91adb0aa302860`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c61328bb6e8a51d4176947cd19babf2660d872019ebb375fcac3c964f4d0bd`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04bcc5c65d2d12a1fbdeaf18184f5dee656aa0335ffbc70660fb526d5dc0c2`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3001db7818ba5ecfa3d8a02faf041ccb1c8a9035c947f48cd045d86e23724`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81cff48308bcf6bd0f2109bd09c0cb34f144b2dfba962ffbe1db73adaa08044`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 307.8 KB (307776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e8f8449020b921f999cd4b0b3e93e958938b8dbcfc9db331855ffea48129fa`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.0-beta.3-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:279ca20d65d1a0dbf40b1604d3a452b33cb7ce2bc873b50ab7a5ff9349c5dcc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332992838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e7d089abaf2c47a1371b6cc08e96e8e2f8d24eec70f8e795c1b33e41c41c42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:22:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 07 Sep 2022 21:22:56 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:23:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e1b60bb8faa2b88e40485b4a95dbd576e24907679b05de0c78362dec9fd5ed96d5ece4a141cf73a20909749b765832c51d2c5b31a59a77913d6db2ae40d3fd9e')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 07 Sep 2022 21:23:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 07 Sep 2022 21:23:25 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 07 Sep 2022 21:23:25 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:23:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:23:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:23:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:23:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:23:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:23:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:23:33 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:23:34 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:23:35 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:23:35 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:23:51 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:23:51 GMT
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
	-	`sha256:e800f51c3128d9d98f99292311d8cfcf6aff80006f7a8610b980ead884f65a29`  
		Last Modified: Wed, 07 Sep 2022 21:27:52 GMT  
		Size: 643.9 KB (643929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9d35750bde1d736e80bee43c0544e38865aba250a2ac6b3c428e4497b5e9`  
		Last Modified: Wed, 07 Sep 2022 21:27:51 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e096b81de1a3f7284446be0432af41a5b4b58a5b456874bb7886de96b97045`  
		Last Modified: Wed, 07 Sep 2022 21:27:55 GMT  
		Size: 15.1 MB (15073702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8afff9325d899befdf790febe8d6142cd1e008afb2aff0fb176e1711c8e024`  
		Last Modified: Wed, 07 Sep 2022 21:27:51 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f35a82d111caffaec6bafc59ea718c162bc2ae84c7d634c033081c07972f9f3`  
		Last Modified: Wed, 07 Sep 2022 21:27:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1ec7808f718b2ac365a0c5af7d09c075a2d3f75020b3d3db706ac4425edfaf`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ebcd9bfe65cef6c4975d67ebf7b37c35b48b5046eb4e5581e77c354b9349b`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de39d1b5849b53cc129cd72b574ce78b52ca0dba835ab46a98a166ccdb2e02fd`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf11f1b9544e317d2e09673b919829f493568d4ffb8236b7c2105bda0f52169`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c698e9f047b2d855747c32d2e660afc04a04c9570624fd7f792fe060b0f08c61`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d44eaacad0442a25d182c0faf18fcefc6b0c02b327561dd3d2df32401a4b0c6`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c186860413e353a19dfb7f22b1d48869e7e720c7ab0508da3f105093e6fe9975`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268b1ccdf4a335813076c750d368ab8f04db9534b2b5e454c494ee776db1170d`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b02eaa6ac31096cc6562add0004b5fe5fa82e59219a3ee730adf10cec446ce`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff70701765ddae8ec2dc248ceaf0c3c97120f51a735849f66862a5eb86cb716`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4625089d3ed10e20d572f2eddd8bf4169910d1ed63d57c4030be559b05da75`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf421c38a1a3e7743511ebabb7d28c7319fd0965e26754e37cea36165c40140`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f32c77ce0b1df0939a5f81dcbf90048c1e73dc9c95104b3fb56e8e6f5783ef`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 362.0 KB (362019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e4a21c72bbb60e33f61928df738e312a1dd374ad361df032542d4fa0c77c6`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-windowsservercore-1809`

```console
$ docker pull caddy@sha256:86c7c66544b35402130c12ec22b24da6217d761850e07ad7c1b76d566789336a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2.6.0-beta.3-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:88e9a60ea5b406bb189949479b4ae063a3cc4daf346989907c2685e65f555a8c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693256192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9797018ab22bc8f72282f5831dc6d9daf160a4b8b12adb24bce2e415c8ffa202`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:20:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 07 Sep 2022 21:20:07 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:21:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e1b60bb8faa2b88e40485b4a95dbd576e24907679b05de0c78362dec9fd5ed96d5ece4a141cf73a20909749b765832c51d2c5b31a59a77913d6db2ae40d3fd9e')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 07 Sep 2022 21:21:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 07 Sep 2022 21:21:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 07 Sep 2022 21:21:21 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:21:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:21:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:21:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:21:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:21:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:21:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:21:28 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:21:29 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:21:30 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:21:31 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:22:19 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:22:19 GMT
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
	-	`sha256:20a7620fe7390d1e63d1e62399c0e75ccb38893e7837c15ac7ba90408cc83f86`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 372.8 KB (372752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d876e92cdae5cc8ef8f030e1935cad493e3d813cb760e327fd3baede311dcfe`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463ae40d7b2aa49884fc8d8ed3005a6dd425600114d2e728dbfc614f584512aa`  
		Last Modified: Wed, 07 Sep 2022 21:27:38 GMT  
		Size: 14.8 MB (14838866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36767dc50f67b8b76415cb0e3e7e76c41358fba6d43a46a82b51c84f7fcca412`  
		Last Modified: Wed, 07 Sep 2022 21:27:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30153786541aece4c50cd4feaf07ac1e53a36f4a8e6a8a630d76285b9653634`  
		Last Modified: Wed, 07 Sep 2022 21:27:33 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8507b8c34256d6baae79684ecc2b03d398caca3141f9da66f8026b30deb12085`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af74df38a1b632249cb4597afc4bffad364f4e30db87382262add3da672756`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d10ae4de6601a9309c0dba410a9cfbb82301be4d4a0f315d2b4c5f8a6210ca`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49cbbe83dc124d1b3f86656793dbfdba968f3900533b6b29da8b7343254a526`  
		Last Modified: Wed, 07 Sep 2022 21:27:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab2e6b2e3f90f097c2155b5c40857c0d7c4283e1c0eafbb19f5fdea9db65cf`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa660547951fe9bc7670499947a22cbf88adb57999e85516eafef4f6ff659a12`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021b454c8d55b873abaee3ab57fe8cfb39d0118ee38ce18298d3769eb8dbe3f5`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67b8e44a69ddb26dfda0a5fda5de1089ab0dfb8df3048a7f1aa1899c477b39`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1e328f7bcf589db46bfe005176f9d34d5916ed38496fb02e91adb0aa302860`  
		Last Modified: Wed, 07 Sep 2022 21:27:30 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c61328bb6e8a51d4176947cd19babf2660d872019ebb375fcac3c964f4d0bd`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04bcc5c65d2d12a1fbdeaf18184f5dee656aa0335ffbc70660fb526d5dc0c2`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3001db7818ba5ecfa3d8a02faf041ccb1c8a9035c947f48cd045d86e23724`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81cff48308bcf6bd0f2109bd09c0cb34f144b2dfba962ffbe1db73adaa08044`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 307.8 KB (307776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e8f8449020b921f999cd4b0b3e93e958938b8dbcfc9db331855ffea48129fa`  
		Last Modified: Wed, 07 Sep 2022 21:27:28 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:1a103be75e722f5949e1b999c1990cf2c6fee2472f6d8f3b9d246a4048d9181d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2.6.0-beta.3-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:279ca20d65d1a0dbf40b1604d3a452b33cb7ce2bc873b50ab7a5ff9349c5dcc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332992838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e7d089abaf2c47a1371b6cc08e96e8e2f8d24eec70f8e795c1b33e41c41c42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:22:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 07 Sep 2022 21:22:56 GMT
ENV CADDY_VERSION=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:23:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0-beta.3/caddy_2.6.0-beta.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e1b60bb8faa2b88e40485b4a95dbd576e24907679b05de0c78362dec9fd5ed96d5ece4a141cf73a20909749b765832c51d2c5b31a59a77913d6db2ae40d3fd9e')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 07 Sep 2022 21:23:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 07 Sep 2022 21:23:25 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 07 Sep 2022 21:23:25 GMT
LABEL org.opencontainers.image.version=v2.6.0-beta.3
# Wed, 07 Sep 2022 21:23:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 07 Sep 2022 21:23:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 07 Sep 2022 21:23:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 07 Sep 2022 21:23:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 07 Sep 2022 21:23:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 07 Sep 2022 21:23:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 07 Sep 2022 21:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 07 Sep 2022 21:23:33 GMT
EXPOSE 80
# Wed, 07 Sep 2022 21:23:34 GMT
EXPOSE 443
# Wed, 07 Sep 2022 21:23:35 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:23:35 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:23:51 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:23:51 GMT
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
	-	`sha256:e800f51c3128d9d98f99292311d8cfcf6aff80006f7a8610b980ead884f65a29`  
		Last Modified: Wed, 07 Sep 2022 21:27:52 GMT  
		Size: 643.9 KB (643929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9d35750bde1d736e80bee43c0544e38865aba250a2ac6b3c428e4497b5e9`  
		Last Modified: Wed, 07 Sep 2022 21:27:51 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e096b81de1a3f7284446be0432af41a5b4b58a5b456874bb7886de96b97045`  
		Last Modified: Wed, 07 Sep 2022 21:27:55 GMT  
		Size: 15.1 MB (15073702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8afff9325d899befdf790febe8d6142cd1e008afb2aff0fb176e1711c8e024`  
		Last Modified: Wed, 07 Sep 2022 21:27:51 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f35a82d111caffaec6bafc59ea718c162bc2ae84c7d634c033081c07972f9f3`  
		Last Modified: Wed, 07 Sep 2022 21:27:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1ec7808f718b2ac365a0c5af7d09c075a2d3f75020b3d3db706ac4425edfaf`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ebcd9bfe65cef6c4975d67ebf7b37c35b48b5046eb4e5581e77c354b9349b`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de39d1b5849b53cc129cd72b574ce78b52ca0dba835ab46a98a166ccdb2e02fd`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf11f1b9544e317d2e09673b919829f493568d4ffb8236b7c2105bda0f52169`  
		Last Modified: Wed, 07 Sep 2022 21:27:49 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c698e9f047b2d855747c32d2e660afc04a04c9570624fd7f792fe060b0f08c61`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d44eaacad0442a25d182c0faf18fcefc6b0c02b327561dd3d2df32401a4b0c6`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c186860413e353a19dfb7f22b1d48869e7e720c7ab0508da3f105093e6fe9975`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268b1ccdf4a335813076c750d368ab8f04db9534b2b5e454c494ee776db1170d`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b02eaa6ac31096cc6562add0004b5fe5fa82e59219a3ee730adf10cec446ce`  
		Last Modified: Wed, 07 Sep 2022 21:27:47 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff70701765ddae8ec2dc248ceaf0c3c97120f51a735849f66862a5eb86cb716`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4625089d3ed10e20d572f2eddd8bf4169910d1ed63d57c4030be559b05da75`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf421c38a1a3e7743511ebabb7d28c7319fd0965e26754e37cea36165c40140`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f32c77ce0b1df0939a5f81dcbf90048c1e73dc9c95104b3fb56e8e6f5783ef`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 362.0 KB (362019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e4a21c72bbb60e33f61928df738e312a1dd374ad361df032542d4fa0c77c6`  
		Last Modified: Wed, 07 Sep 2022 21:27:45 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:b31ff95e98737b849d6af1fb9d9cb54a66ba3684564b3310541f60b12b1dd619
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
$ docker pull caddy@sha256:cfa7d94aa1f0c68a167b147a8573711283df2cd6fc285d220387f20206ff4874
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83af79bf9e25fcac6c74f9e4862c41808daae08fc9693798b23edb747e6e938`
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
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:22 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:22 GMT
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
$ docker pull caddy@sha256:ab90c32af49182ef7512475520559c58882dc9c3eb856bd05045845355bf5b70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499d71de73836366f4be3ee44abf878f97102a0f242d2afb55a1238073b79b6`
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
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:21 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:21 GMT
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
$ docker pull caddy@sha256:7981b1b833894ee4cde9129ba6181dd80307b7e1df3ecd18b9720d88993e1c27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a985003f9f6cbce93bc66be158b0f622194e08f2b1ee5a8eba5cc793446602b`
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
# Wed, 07 Sep 2022 20:57:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:23 GMT
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
$ docker pull caddy@sha256:03f7dc5da8bd904d5942283fe31d401249560bb74b0dbfd88eba3c65e5ef9493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea1482cd071f0d18c0519a9b6819e949540f0e761ed8645f95060c4917f7c0`
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
# Wed, 07 Sep 2022 20:39:31 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:39:32 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:39:33 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:39:34 GMT
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
$ docker pull caddy@sha256:c98b27fc9159cf13c479d2052080ca25cfcbe5546cfe258c1a6f70827801f6e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d851d72b6e66e7190c29af3b6f08ff07e0372c054fbc46ae13ad4f38f9554e`
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
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:24 GMT
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
$ docker pull caddy@sha256:8147dd7b152004aa641f7699109649703831e18dc563fbb6448d54e88ef94766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7460051eff8773d7f2c072637754453656be2c21c74f71711669c5ab9bbba9`
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
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:28 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:29 GMT
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
$ docker pull caddy@sha256:1a8f153ebe56283c4d5168d92c049b00ae1c635248f99295c4c106ccfad3012f
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

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:35d5468f9f5b642625cd0db6ac93f5fb012037c4783516a2db9ee1f9942a5f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126581869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446a17d6179d93d6f4f576b01e0d83b0271aae295f07c5e1fdb031f1af9bdbba`
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
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:25 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:27 GMT
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
	-	`sha256:39a0d8604657ba9022aa5b88de3771f9a87f7a100187743f8b02c4995137f7c7`  
		Last Modified: Wed, 07 Sep 2022 21:20:09 GMT  
		Size: 1.2 MB (1215200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf75964ac643c8e0de2048260f7080c9a9afd12c87c3f93305892303c02626`  
		Last Modified: Wed, 07 Sep 2022 21:20:08 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:52932e74f09f4f600395ef0e65ac7761f74590c784de385b329c3deba73e9728
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122585761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceffdb3edb815118e8e62d2de89c304f5c9789a479a4aa646137643225c71277`
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
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:30 GMT
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
	-	`sha256:714c3b82fd5725d5c508bf921d8e44a826b6e80b7cf80206371441629020f7df`  
		Last Modified: Wed, 07 Sep 2022 20:50:44 GMT  
		Size: 1.2 MB (1162989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b035ad2bb7133b1e1f29d51c79911610b64ce645964402e0303856cc02a489d6`  
		Last Modified: Wed, 07 Sep 2022 20:50:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d54381d61daa9bbeb03bcbaa1c9fbf5e4890cd3f23fc2aebc13bb763bcd78efe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121421388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2fbb736245edf10b20547bdda39806040da01b5ed7daad738d04767e91fd47`
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
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:57:33 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:57:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:57:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:57:35 GMT
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
	-	`sha256:068f91f2941da883f37d54e440827226340fd3cad687e8529e236e235400c098`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 1.2 MB (1159978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae346762b582e00a5f229e741b110848ff0c3b95a30e95e56d235d7eed3c31`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e4ced291a901313117012e281dd0de28ec1d3c2e70246002d0533aea698925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121532298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3045db8e0202ea02304fde36f24f2fa1f10473c6b30d8dd9cc85392b3e63eab`
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
# Wed, 07 Sep 2022 20:39:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:39:42 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:39:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:39:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:39:46 GMT
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
	-	`sha256:5340d2088ba2060ab6fd7ac03124f5c7f395a51670305bf90a89da96988e8daa`  
		Last Modified: Wed, 07 Sep 2022 20:41:12 GMT  
		Size: 1.1 MB (1120446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5c4ba17c8241ba8dfbe915956db306ef689730489ef97462e99e641a0c1bf`  
		Last Modified: Wed, 07 Sep 2022 20:41:11 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:2cc10ae309cb5fac54e5e8d39dbef0f535d8ad5336c9b32415250274fcc0cfb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122072737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8c0fd8624128c41541d92222a799f89ca10620bd3b187579c1c6cba4827192`
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
# Wed, 07 Sep 2022 21:16:31 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:32 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:16:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:16:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:16:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:16:35 GMT
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
	-	`sha256:fdb755156f20625cf7436ebf9dd3e9d73ed62942073cbc911c4f42e739412d51`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 1.1 MB (1103854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be64bd7379e703449226d281d2a47bfacaf4193e886ff12bd078fa95dd5823f`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:ef06f5dd643bb6af248afc42b5a46c88c13404a0b8718cf9ab9e5b07a36e6c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b9e4f098357534de1347fdb9b83e146abab58747e67d367d7e39f967d47b3a`
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
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:41:37 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:41:38 GMT
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
	-	`sha256:b6163d00c71b4379b800d1de8c81291389a7c79cc6d574dcce5e37183b3afde4`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 1.2 MB (1167442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532161760fe5ac59a0240e62f0bc251ea4e8de1f539811850f43e3802394e34`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:7a5223f7720e5df685236b56c58dd57fad525b88fdb76e56e121a9e3be273615
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2494943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ea73be5cb10a5570dad83431d3aba123ed40e564b9f20fbf123f2be4546100`
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
# Wed, 07 Sep 2022 21:18:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:18:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:18:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:57 GMT
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
	-	`sha256:ff9d42bb565792710d4018b199ac636b9be0ffb9db23b35bc1eee69dca771c33`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61760b64ebc2bb823a7baca5dd0c0d7db3befbbed5ad1a8c1a5e6eaf346ca0b4`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f87d92375e5d9779ea8a646f053e96096f690a3c73617055f862f173f5033`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3271b3d777871daea415771bcf19be13bdf3d9fcd47e5c1777c9f480790716e`  
		Last Modified: Wed, 07 Sep 2022 21:27:15 GMT  
		Size: 1.9 MB (1868000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b438765ca79769b19f152009561021f6f8ac5c4446b1fc99e7fd9b10a4e8adba`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:1fb3a7ef40462a897a1a3b8ed772a24cfc804cd63942b33130cd129a188cccd2
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
$ docker pull caddy@sha256:35d5468f9f5b642625cd0db6ac93f5fb012037c4783516a2db9ee1f9942a5f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126581869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446a17d6179d93d6f4f576b01e0d83b0271aae295f07c5e1fdb031f1af9bdbba`
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
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:19:25 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:19:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:19:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:19:27 GMT
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
	-	`sha256:39a0d8604657ba9022aa5b88de3771f9a87f7a100187743f8b02c4995137f7c7`  
		Last Modified: Wed, 07 Sep 2022 21:20:09 GMT  
		Size: 1.2 MB (1215200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf75964ac643c8e0de2048260f7080c9a9afd12c87c3f93305892303c02626`  
		Last Modified: Wed, 07 Sep 2022 21:20:08 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:52932e74f09f4f600395ef0e65ac7761f74590c784de385b329c3deba73e9728
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122585761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceffdb3edb815118e8e62d2de89c304f5c9789a479a4aa646137643225c71277`
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
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:49:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:49:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:49:30 GMT
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
	-	`sha256:714c3b82fd5725d5c508bf921d8e44a826b6e80b7cf80206371441629020f7df`  
		Last Modified: Wed, 07 Sep 2022 20:50:44 GMT  
		Size: 1.2 MB (1162989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b035ad2bb7133b1e1f29d51c79911610b64ce645964402e0303856cc02a489d6`  
		Last Modified: Wed, 07 Sep 2022 20:50:43 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d54381d61daa9bbeb03bcbaa1c9fbf5e4890cd3f23fc2aebc13bb763bcd78efe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121421388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2fbb736245edf10b20547bdda39806040da01b5ed7daad738d04767e91fd47`
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
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:57:33 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:57:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:57:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:57:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:57:35 GMT
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
	-	`sha256:068f91f2941da883f37d54e440827226340fd3cad687e8529e236e235400c098`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 1.2 MB (1159978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae346762b582e00a5f229e741b110848ff0c3b95a30e95e56d235d7eed3c31`  
		Last Modified: Wed, 07 Sep 2022 20:59:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e4ced291a901313117012e281dd0de28ec1d3c2e70246002d0533aea698925b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121532298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3045db8e0202ea02304fde36f24f2fa1f10473c6b30d8dd9cc85392b3e63eab`
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
# Wed, 07 Sep 2022 20:39:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:39:42 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:39:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:39:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:39:46 GMT
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
	-	`sha256:5340d2088ba2060ab6fd7ac03124f5c7f395a51670305bf90a89da96988e8daa`  
		Last Modified: Wed, 07 Sep 2022 20:41:12 GMT  
		Size: 1.1 MB (1120446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f5c4ba17c8241ba8dfbe915956db306ef689730489ef97462e99e641a0c1bf`  
		Last Modified: Wed, 07 Sep 2022 20:41:11 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:2cc10ae309cb5fac54e5e8d39dbef0f535d8ad5336c9b32415250274fcc0cfb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122072737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8c0fd8624128c41541d92222a799f89ca10620bd3b187579c1c6cba4827192`
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
# Wed, 07 Sep 2022 21:16:31 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:32 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:16:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:16:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 21:16:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 21:16:35 GMT
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
	-	`sha256:fdb755156f20625cf7436ebf9dd3e9d73ed62942073cbc911c4f42e739412d51`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 1.1 MB (1103854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be64bd7379e703449226d281d2a47bfacaf4193e886ff12bd078fa95dd5823f`  
		Last Modified: Wed, 07 Sep 2022 21:17:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ef06f5dd643bb6af248afc42b5a46c88c13404a0b8718cf9ab9e5b07a36e6c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b9e4f098357534de1347fdb9b83e146abab58747e67d367d7e39f967d47b3a`
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
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 20:41:37 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 20:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 20:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 07 Sep 2022 20:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 07 Sep 2022 20:41:38 GMT
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
	-	`sha256:b6163d00c71b4379b800d1de8c81291389a7c79cc6d574dcce5e37183b3afde4`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 1.2 MB (1167442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532161760fe5ac59a0240e62f0bc251ea4e8de1f539811850f43e3802394e34`  
		Last Modified: Wed, 07 Sep 2022 20:42:50 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fc7d6643b94f172dc0be1c2a55fe404556c0ef4308cd01485587e677fd69b58f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
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
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5bd4a15f1f1608bda512eef3fb6ab85a621321eaf331befc3460e95e84bbdfc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:7a5223f7720e5df685236b56c58dd57fad525b88fdb76e56e121a9e3be273615
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2494943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ea73be5cb10a5570dad83431d3aba123ed40e564b9f20fbf123f2be4546100`
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
# Wed, 07 Sep 2022 21:18:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:18:29 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:18:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:57 GMT
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
	-	`sha256:ff9d42bb565792710d4018b199ac636b9be0ffb9db23b35bc1eee69dca771c33`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61760b64ebc2bb823a7baca5dd0c0d7db3befbbed5ad1a8c1a5e6eaf346ca0b4`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f87d92375e5d9779ea8a646f053e96096f690a3c73617055f862f173f5033`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3271b3d777871daea415771bcf19be13bdf3d9fcd47e5c1777c9f480790716e`  
		Last Modified: Wed, 07 Sep 2022 21:27:15 GMT  
		Size: 1.9 MB (1868000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b438765ca79769b19f152009561021f6f8ac5c4446b1fc99e7fd9b10a4e8adba`  
		Last Modified: Wed, 07 Sep 2022 21:27:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:c2aa034bd91237e02c80e030f1366fe0e20c88dfc6b9eac5c3cfefdc447b7bc9
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
$ docker pull caddy@sha256:cfa7d94aa1f0c68a167b147a8573711283df2cd6fc285d220387f20206ff4874
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83af79bf9e25fcac6c74f9e4862c41808daae08fc9693798b23edb747e6e938`
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
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:19:22 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:19:22 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:19:22 GMT
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
$ docker pull caddy@sha256:ab90c32af49182ef7512475520559c58882dc9c3eb856bd05045845355bf5b70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499d71de73836366f4be3ee44abf878f97102a0f242d2afb55a1238073b79b6`
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
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:49:21 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:49:21 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:49:21 GMT
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
$ docker pull caddy@sha256:7981b1b833894ee4cde9129ba6181dd80307b7e1df3ecd18b9720d88993e1c27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a985003f9f6cbce93bc66be158b0f622194e08f2b1ee5a8eba5cc793446602b`
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
# Wed, 07 Sep 2022 20:57:22 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:57:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:57:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:57:23 GMT
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
$ docker pull caddy@sha256:03f7dc5da8bd904d5942283fe31d401249560bb74b0dbfd88eba3c65e5ef9493
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea1482cd071f0d18c0519a9b6819e949540f0e761ed8645f95060c4917f7c0`
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
# Wed, 07 Sep 2022 20:39:31 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:39:32 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:39:33 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:39:34 GMT
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
$ docker pull caddy@sha256:c98b27fc9159cf13c479d2052080ca25cfcbe5546cfe258c1a6f70827801f6e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d851d72b6e66e7190c29af3b6f08ff07e0372c054fbc46ae13ad4f38f9554e`
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
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:23 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:23 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 21:16:24 GMT
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
$ docker pull caddy@sha256:8147dd7b152004aa641f7699109649703831e18dc563fbb6448d54e88ef94766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7460051eff8773d7f2c072637754453656be2c21c74f71711669c5ab9bbba9`
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
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 20:41:28 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 20:41:28 GMT
WORKDIR /srv
# Wed, 07 Sep 2022 20:41:29 GMT
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
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:e93223c9604a42ed32a365ac8f0a2cb429b636c5cd64417763033237d281936d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:8e736a0201648378f698716a66fc532320d11f8357cb58773c47b5cfe6cfed3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:c91a990b986a36c2543b5564ff2b3c9d12a5a40dd29ae191459d72ee6f20d53e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692666689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb824755e59757ce9bf9128a91532631b0098c97f76df4c7362c78e9a95e2af`
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
# Wed, 07 Sep 2022 21:15:06 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:15:07 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:11 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:12 GMT
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
	-	`sha256:57ce01e7e268cbbda2699ce432adec3a3b9ecd6803bcf4938d027eed47a3af8a`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7bcddeb248b5e14abd5260b3522729a92daf80ff57e83f06297a18490d1c29`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472b4a94bf17586618586117d5b6cc4dea2f95b7d059e1dd9a4b2a08e625eb3`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 329.3 KB (329253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa363794df9fdf8a3314512719bd1b4d85f7c50b05abe35251454b41f388425e`  
		Last Modified: Wed, 07 Sep 2022 21:26:26 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e43f46a4015c9bdce6f65c400e02eca5ae6d1a642bfc498c1c231e8d60a8958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:acb38c4949393573deea1027f9359d1d71cba9688861af508d0ca5fa4a27fe11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332395153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9895f9c4cd6562c1f04916dd26f5ff5f38c489f512d3b35a73027c426703410`
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
# Wed, 07 Sep 2022 21:16:19 GMT
EXPOSE 443/udp
# Wed, 07 Sep 2022 21:16:20 GMT
EXPOSE 2019
# Wed, 07 Sep 2022 21:16:43 GMT
RUN caddy version
# Wed, 07 Sep 2022 21:16:45 GMT
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
	-	`sha256:57c1fcec7d768d724002bc5152c45047d93da78645c21cd14528d4780a1dd0b8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891af5f2764aec17e6ed3a9eb428d22c80977052dc17bdfcea60022736202af8`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3ce21f1a0574a33add99ef62cd477a0ce21979683574c32c5882a3ba2d220`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 365.3 KB (365254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628e2e919028074fd4499bbab5b728d17ff7db91c44a4e9889940da6e19c39db`  
		Last Modified: Wed, 07 Sep 2022 21:26:40 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
