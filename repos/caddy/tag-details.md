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
$ docker pull caddy@sha256:343a268d45b94fb60575c5a477f4cf3a62b24e1c1dc6c63a25488c4871c98c69
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
$ docker pull caddy@sha256:2bd3f77e2d21db96ae5a1decdb8df220d98b96e7b812cf7d368828b16bf65ae6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99e5e593f69a4c70d75271117799e5796754e07429560f8f70a6a62a9c09b8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 07:46:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 07:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 07:46:54 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 07:46:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 07:46:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 07:46:58 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 07:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195e97acbd9f5678e292401c0fae3db777aff49e77f38d9cc3f101265b4cdf43`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 291.6 KB (291593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b702741191d81f669709a2af927df34f91029d7bdee74215cf2c65f2270cd`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6330f4d2e50b7bf2126496a3e12ab164af1ad5972222a6dd6ad58fd449b11fe`  
		Last Modified: Wed, 13 Jul 2022 07:47:23 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acec8070f9fa557cb093f66f0b2af0db792a0452918c52d5528fcb4588ad492`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:71bdbcc7ee7d24783e2cf57be294f8c15b313f9c24f41ee4bf4f442c97dc8ba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b22970098c4484f2b4a2c0d563cd0856a595d830bf660a6790517a3e6dc0c04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 00:24:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 00:24:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 00:24:47 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:24:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 00:24:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 00:24:54 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 00:24:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 00:24:59 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 00:24:59 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 00:25:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c75bf2949196f38f164b182514870806879c33b90ec192cdedc33beb7164f3`  
		Last Modified: Wed, 13 Jul 2022 00:26:20 GMT  
		Size: 291.8 KB (291823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e9fed1085fb888faddfae5023a802bb85f365cfde9aacc7b2cf25064c0a7d`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d79f4f39a3e95ed2ada99510758a8816e4ddcf160793887df642ea34d47d6`  
		Last Modified: Wed, 13 Jul 2022 00:26:28 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099d09b43e9c3fdfbe6250cc5340915853372077bf3606d33ba1b9c5bad5c38`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1db5af09e7e93ccc64f39d2aefa6438f3346a62fff17d5f006eef3bf5541424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3d980491df522f57fa63138e24e8c6be022acb10104bab97857a4eab9d04f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 14 Jul 2022 04:50:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 14 Jul 2022 04:50:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 14 Jul 2022 04:50:42 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Jul 2022 04:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 80
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 443
# Thu, 14 Jul 2022 04:50:55 GMT
EXPOSE 2019
# Thu, 14 Jul 2022 04:50:55 GMT
WORKDIR /srv
# Thu, 14 Jul 2022 04:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d2eab8b066328ae05bd108fd3d593cfea00c0c5b4a920788ae29400dfa4fc`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 290.8 KB (290762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e007f0123b4d81f10149eb27d05581180511d1b2884e9f286496e20935f56453`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35e23b17501f974f98785b56b4286fedfcb3e968b0564292daec9ecd9451e`  
		Last Modified: Thu, 14 Jul 2022 04:52:27 GMT  
		Size: 13.3 MB (13347758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbc25b5d1376069d3e359ea4fb05678d63a4a0d20fdce60afc005cfbf344e9`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e277f1e570bb65d07ca7ddaf11bd50b8f64643b579e2a1500165d0d10e873b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15720992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ab296123268f045db4f04fdd9542ea39cf0869b8a5790b52e8359cf4301f2f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 09:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 09:10:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 09:10:27 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 09:10:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 09:10:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 09:10:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 09:10:33 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 09:10:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 09:10:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 09:10:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 09:10:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 09:10:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 09:10:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 09:10:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 09:10:41 GMT
EXPOSE 80
# Wed, 13 Jul 2022 09:10:42 GMT
EXPOSE 443
# Wed, 13 Jul 2022 09:10:43 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 09:10:44 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 09:10:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e2632fbf469bd4459a122146d4f5c544524b9917ebbb1c82ca604c846e6d03`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 291.5 KB (291462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136b5c9b9f23df66b6049078ee2f4df8231ed7eb7f543cc31055c0c338074a3`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d759768dee9c2f0e5c5353760cb5d7fdb641c3bbc7160a9ef0e1428a504a820b`  
		Last Modified: Wed, 13 Jul 2022 09:11:30 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f38216dc74dd3541e3282c41fd26512f9161bbc74eb0fef8374f88c07c33f`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:8bf33283df3ab62c0987b87b518be60e587e8e8f492f9001c9f513126218c3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b6dd61b467dc78c47f12742f5af2367935a9ffb8f6dcc8ce8382764c2d1ab8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 22:09:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 22:09:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 22:09:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:10:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 22:10:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 22:10:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 22:10:18 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 22:10:21 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 22:10:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 22:10:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 22:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 22:10:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 22:10:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 22:10:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 22:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 22:10:40 GMT
EXPOSE 80
# Wed, 13 Jul 2022 22:10:43 GMT
EXPOSE 443
# Wed, 13 Jul 2022 22:10:44 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 22:10:48 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 22:10:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49126cc0b1f1c1e51c05b6d7443ed73b5fd2577d177ced4eb36ba827a6b9e68c`  
		Last Modified: Wed, 13 Jul 2022 22:12:19 GMT  
		Size: 293.9 KB (293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f5f92095cf2a8c6afe25b29ea21344778855b89f160fed628effd01704c1c2`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12fbf7d78c1725ab5956092ae9577b979994dc526cbd9f8368c69ce317b692`  
		Last Modified: Wed, 13 Jul 2022 22:12:21 GMT  
		Size: 12.3 MB (12309531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905929de5f23fe3fc6a3b51fc5e5ae5d69bb42d68a20069887fbae365e82fba`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:f3f1634a0c819eb255025ed4f6ed0cf373cf040b4433b99e741b9f356c24f035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db99049e35d90916167a13c53576818e74e4b0f30b57123b9f866b7712c8305b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 12:22:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 12:22:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 12:22:45 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:22:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 12:22:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 12:22:50 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 12:22:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 12:22:53 GMT
EXPOSE 80
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 443
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 12:22:54 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 12:22:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a278a0c4f266219ec8afd82734a3a15f7ad274e786c5e813adde536d23e7a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 291.9 KB (291943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bfcbf66ce9f538fed4132cec8e97597e9ace9340502c5ed98c06909e9369c9`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26380b79ed6fa2324d957b5d5f3c38ae3aaccb280e477850bdae2952a1e1c308`  
		Last Modified: Wed, 13 Jul 2022 12:23:44 GMT  
		Size: 13.5 MB (13460701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319ee79626cacd3ef26113bfb7c3a9086642a88ba734de13a93138ce13b839a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 155.0 B  
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
$ docker pull caddy@sha256:2db1d5975a0e02f6d4ce83d5ff02287989fc3478190a4027aa7c583e0f63e418
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
$ docker pull caddy@sha256:2bd3f77e2d21db96ae5a1decdb8df220d98b96e7b812cf7d368828b16bf65ae6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99e5e593f69a4c70d75271117799e5796754e07429560f8f70a6a62a9c09b8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 07:46:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 07:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 07:46:54 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 07:46:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 07:46:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 07:46:58 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 07:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195e97acbd9f5678e292401c0fae3db777aff49e77f38d9cc3f101265b4cdf43`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 291.6 KB (291593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b702741191d81f669709a2af927df34f91029d7bdee74215cf2c65f2270cd`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6330f4d2e50b7bf2126496a3e12ab164af1ad5972222a6dd6ad58fd449b11fe`  
		Last Modified: Wed, 13 Jul 2022 07:47:23 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acec8070f9fa557cb093f66f0b2af0db792a0452918c52d5528fcb4588ad492`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:71bdbcc7ee7d24783e2cf57be294f8c15b313f9c24f41ee4bf4f442c97dc8ba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b22970098c4484f2b4a2c0d563cd0856a595d830bf660a6790517a3e6dc0c04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 00:24:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 00:24:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 00:24:47 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:24:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 00:24:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 00:24:54 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 00:24:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 00:24:59 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 00:24:59 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 00:25:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c75bf2949196f38f164b182514870806879c33b90ec192cdedc33beb7164f3`  
		Last Modified: Wed, 13 Jul 2022 00:26:20 GMT  
		Size: 291.8 KB (291823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e9fed1085fb888faddfae5023a802bb85f365cfde9aacc7b2cf25064c0a7d`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d79f4f39a3e95ed2ada99510758a8816e4ddcf160793887df642ea34d47d6`  
		Last Modified: Wed, 13 Jul 2022 00:26:28 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099d09b43e9c3fdfbe6250cc5340915853372077bf3606d33ba1b9c5bad5c38`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1db5af09e7e93ccc64f39d2aefa6438f3346a62fff17d5f006eef3bf5541424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3d980491df522f57fa63138e24e8c6be022acb10104bab97857a4eab9d04f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 14 Jul 2022 04:50:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 14 Jul 2022 04:50:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 14 Jul 2022 04:50:42 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Jul 2022 04:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 80
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 443
# Thu, 14 Jul 2022 04:50:55 GMT
EXPOSE 2019
# Thu, 14 Jul 2022 04:50:55 GMT
WORKDIR /srv
# Thu, 14 Jul 2022 04:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d2eab8b066328ae05bd108fd3d593cfea00c0c5b4a920788ae29400dfa4fc`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 290.8 KB (290762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e007f0123b4d81f10149eb27d05581180511d1b2884e9f286496e20935f56453`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35e23b17501f974f98785b56b4286fedfcb3e968b0564292daec9ecd9451e`  
		Last Modified: Thu, 14 Jul 2022 04:52:27 GMT  
		Size: 13.3 MB (13347758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbc25b5d1376069d3e359ea4fb05678d63a4a0d20fdce60afc005cfbf344e9`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e277f1e570bb65d07ca7ddaf11bd50b8f64643b579e2a1500165d0d10e873b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15720992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ab296123268f045db4f04fdd9542ea39cf0869b8a5790b52e8359cf4301f2f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 09:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 09:10:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 09:10:27 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 09:10:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 09:10:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 09:10:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 09:10:33 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 09:10:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 09:10:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 09:10:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 09:10:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 09:10:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 09:10:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 09:10:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 09:10:41 GMT
EXPOSE 80
# Wed, 13 Jul 2022 09:10:42 GMT
EXPOSE 443
# Wed, 13 Jul 2022 09:10:43 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 09:10:44 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 09:10:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e2632fbf469bd4459a122146d4f5c544524b9917ebbb1c82ca604c846e6d03`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 291.5 KB (291462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136b5c9b9f23df66b6049078ee2f4df8231ed7eb7f543cc31055c0c338074a3`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d759768dee9c2f0e5c5353760cb5d7fdb641c3bbc7160a9ef0e1428a504a820b`  
		Last Modified: Wed, 13 Jul 2022 09:11:30 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f38216dc74dd3541e3282c41fd26512f9161bbc74eb0fef8374f88c07c33f`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8bf33283df3ab62c0987b87b518be60e587e8e8f492f9001c9f513126218c3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b6dd61b467dc78c47f12742f5af2367935a9ffb8f6dcc8ce8382764c2d1ab8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 22:09:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 22:09:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 22:09:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:10:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 22:10:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 22:10:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 22:10:18 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 22:10:21 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 22:10:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 22:10:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 22:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 22:10:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 22:10:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 22:10:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 22:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 22:10:40 GMT
EXPOSE 80
# Wed, 13 Jul 2022 22:10:43 GMT
EXPOSE 443
# Wed, 13 Jul 2022 22:10:44 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 22:10:48 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 22:10:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49126cc0b1f1c1e51c05b6d7443ed73b5fd2577d177ced4eb36ba827a6b9e68c`  
		Last Modified: Wed, 13 Jul 2022 22:12:19 GMT  
		Size: 293.9 KB (293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f5f92095cf2a8c6afe25b29ea21344778855b89f160fed628effd01704c1c2`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12fbf7d78c1725ab5956092ae9577b979994dc526cbd9f8368c69ce317b692`  
		Last Modified: Wed, 13 Jul 2022 22:12:21 GMT  
		Size: 12.3 MB (12309531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905929de5f23fe3fc6a3b51fc5e5ae5d69bb42d68a20069887fbae365e82fba`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f3f1634a0c819eb255025ed4f6ed0cf373cf040b4433b99e741b9f356c24f035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db99049e35d90916167a13c53576818e74e4b0f30b57123b9f866b7712c8305b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 12:22:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 12:22:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 12:22:45 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:22:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 12:22:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 12:22:50 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 12:22:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 12:22:53 GMT
EXPOSE 80
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 443
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 12:22:54 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 12:22:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a278a0c4f266219ec8afd82734a3a15f7ad274e786c5e813adde536d23e7a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 291.9 KB (291943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bfcbf66ce9f538fed4132cec8e97597e9ace9340502c5ed98c06909e9369c9`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26380b79ed6fa2324d957b5d5f3c38ae3aaccb280e477850bdae2952a1e1c308`  
		Last Modified: Wed, 13 Jul 2022 12:23:44 GMT  
		Size: 13.5 MB (13460701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319ee79626cacd3ef26113bfb7c3a9086642a88ba734de13a93138ce13b839a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:f68592219340bb743bb752f7c4c5711a95693066900a45c88ef1a99fd59f7a99
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
$ docker pull caddy@sha256:83d4d0707f0fdf954311174224be106071959f6cadb80a90349f481eae9fb2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126544689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a1b98417a84b3a24a165471d7d84c070cc923dac2d4c9d1f893e347b24d418`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:12 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:01:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 00:01:48 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:01:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:01:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:01:49 GMT
WORKDIR /go
# Wed, 13 Jul 2022 07:47:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 07:47:03 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 07:47:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 07:47:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 07:47:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd112bd56ec3e5c889db16588dbcac85cbd1a95bcc45882e8ac837e2315b5c`  
		Last Modified: Wed, 13 Jul 2022 00:12:05 GMT  
		Size: 115.2 MB (115242817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd2cfe75a75aec6138ba0c67d2af1a7a2dd4c5a3b1bde23967b4caef488acb8`  
		Last Modified: Wed, 13 Jul 2022 00:11:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448905a1cc77d184aea8ebe3718f902d023568b6c2f19a1303f82abe51bedd1`  
		Last Modified: Wed, 13 Jul 2022 07:47:36 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996f6eb2c1beceddac26dd5f2c7ad82b7a99fbfbda5afe10a2a07912cedc13f3`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232bb821e1caea148f02346da5fa5562ce283c3cc15a38b5a5075032d51a21`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:703622cb9f18f0b8afa018cad85ee38f07a589dad0efd9a17320f18ecc13cd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122569995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8bede613e41fb58ab47edf7b489bb233d938d4ecdecac92918e083fb05bc964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:16:58 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:21:00 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:21:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:21:02 GMT
WORKDIR /go
# Tue, 12 Jul 2022 22:56:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 12 Jul 2022 22:56:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 00:25:16 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:25:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 00:25:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 00:25:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 00:25:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a482f319cf9a81f236c51c53bb1c689e8b1fa579667d51ca5ed246ee842f0e`  
		Last Modified: Tue, 12 Jul 2022 22:35:48 GMT  
		Size: 111.7 MB (111655243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9920ad3da4e1bfa17727a4264ec8048f45c5117be4799010b8a718e4004cd91`  
		Last Modified: Tue, 12 Jul 2022 22:34:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afe0ff63358ebff72e63d2f0e98d572f7b7705859c43e57f9ef9cfb8447237`  
		Last Modified: Tue, 12 Jul 2022 22:57:30 GMT  
		Size: 6.8 MB (6806683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8e293f9d738d252bf475ce912e8291238915bf42ce57e839482143ab0287d`  
		Last Modified: Wed, 13 Jul 2022 00:26:43 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5f7917a376356834c38ec70309cec40192a27123e32b1516ccdf50a3de64a`  
		Last Modified: Wed, 13 Jul 2022 00:26:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4d18ee072281fc258a9eb19957ead3c8465339eb7b1f5f269afdb3bc9ad4fa09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121402125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6e75b9e1db747dea3dc9c073f2ecaffbce977107e2c900a2163fbdb0297969`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:40 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 01:20:33 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:20:36 GMT
WORKDIR /go
# Thu, 14 Jul 2022 04:51:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Jul 2022 04:51:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 14 Jul 2022 04:51:15 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:51:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Jul 2022 04:51:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Jul 2022 04:51:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Jul 2022 04:51:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e1c3c4b2486777cff8d39eaf101ab399597d87ae5c000dd7b7ad510d46797d`  
		Last Modified: Wed, 13 Jul 2022 01:47:48 GMT  
		Size: 111.4 MB (111423439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309d1e7915b7277aa2caa1a4fdae40f2ca49b928d9fec95e663f3a5711b45e6`  
		Last Modified: Wed, 13 Jul 2022 01:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfb02347c7d72c96558b8bb46a4f048d1e45182f13e10c0e83edf22747ea95`  
		Last Modified: Thu, 14 Jul 2022 04:52:44 GMT  
		Size: 6.1 MB (6067337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e3c4142f91b38c3b1e65fd6fb6ef9628dcc3556482e762152e8c9d1d3c20d`  
		Last Modified: Thu, 14 Jul 2022 04:52:42 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686a634185cb5f4c2d9dba579c1eb3beebb78e69bd25447da60ac8409e08766`  
		Last Modified: Thu, 14 Jul 2022 04:52:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:290cfd704a23c2ddcb1f182f2f17674fdcdbeaeb62282475cfaeb2dcaae9af7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e226abb8bbf011ea45e449c5070530a1ef1cc1df8f81f78ffe8324696cdf73d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:25 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:24:55 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:24:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:24:58 GMT
WORKDIR /go
# Wed, 13 Jul 2022 09:10:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 09:10:54 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 09:10:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 09:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 09:11:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 09:11:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c4cc194face1e292d4841acf35c12d3d21a64fe5cfa594ab6dc52873073ab8`  
		Last Modified: Tue, 12 Jul 2022 22:33:47 GMT  
		Size: 110.3 MB (110292574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685667e0af253c6086e8398208c7561561541b211e9ddbbcf4ef6be883686ef`  
		Last Modified: Tue, 12 Jul 2022 22:33:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db124a84d37b8773dd6f7f3dd17698fb5775f4f372998d4594652b36951c51ed`  
		Last Modified: Wed, 13 Jul 2022 09:11:45 GMT  
		Size: 7.1 MB (7051424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ee509a95002753f22f52015b6d73f187734670231017a28315b2e679616d0`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c79b21287a253cbeff92e71a14c553de9540b34d770e268a8516fa4aa873e8`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:45efd91580c564bafa163224d57cea1742c852d9dbcacc2458d07f2766222c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122018553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe6a5f3afb3907fcc50178a016518559167b721a37de228f9c66eb515bf066f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:04:48 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 05:08:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 05:08:16 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 05:08:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:08:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 05:08:32 GMT
WORKDIR /go
# Wed, 13 Jul 2022 22:11:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 22:11:13 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 22:11:14 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:11:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 22:11:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 22:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 22:11:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a10ac130bb3da5c68d2d1ddd0bddd9c9aafed7a843450be82de6d7afbf936b`  
		Last Modified: Wed, 13 Jul 2022 05:39:52 GMT  
		Size: 110.3 MB (110295902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1b6a1686a88fdc83aa69e21aa8af36292281aded76e23d6478ea562dc6f96`  
		Last Modified: Wed, 13 Jul 2022 05:37:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f614e9e2e974dc8b16c5a51ac52e34a0134a1d53aafdb0b3f5cfa4b5d2856fc`  
		Last Modified: Wed, 13 Jul 2022 22:12:38 GMT  
		Size: 7.5 MB (7481646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94763b8678030186e0f46988e42fc162735c88413e46aaf5ed2a4956f39dd44`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea48a0db2f2ebe6c442a9a51b0febfdd54d1baf5924bc7cb12b54ae2011796d`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7903fc94e9870b09a5c16e5ef6afc2ccb73eb64a00028d57a0a8b954c7d36a3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7170749c53aeec1e443a594cab8e6d8ae65cf4dbd937ab548ffaf95dfefedf94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:35:10 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:37:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 04:38:12 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:38:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:38:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:38:14 GMT
WORKDIR /go
# Wed, 13 Jul 2022 12:23:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 12:23:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 12:23:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:23:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 12:23:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 12:23:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 12:23:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0da7506b596726f522d72670637523b1f1601e15dc1dd4cb1be338164021b`  
		Last Modified: Wed, 13 Jul 2022 04:56:57 GMT  
		Size: 113.2 MB (113165463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78cd6c9206bd154e2ee3a37419413d222f10a31c24af3882cbe40c976c6016`  
		Last Modified: Wed, 13 Jul 2022 04:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15666b0ca68b6455e83f584a5eb1e817b064585023d7a42f80f62a857ae83ec9`  
		Last Modified: Wed, 13 Jul 2022 12:23:56 GMT  
		Size: 7.1 MB (7052809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa673a9dcaa66c8c1003f2b6df47b953e6e58b37233265f1949e78286795d385`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 1.2 MB (1243127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a95a05c45b1aa5d96976995433e8b8a21d81800acaf6535149cdfd51817d5ca`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:e6697d7888f6b3af8a07ad6f89ba4f7a556aad9b22e17a36fbc9d57146b82a99
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
$ docker pull caddy@sha256:83d4d0707f0fdf954311174224be106071959f6cadb80a90349f481eae9fb2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126544689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a1b98417a84b3a24a165471d7d84c070cc923dac2d4c9d1f893e347b24d418`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:12 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:01:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 00:01:48 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:01:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:01:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:01:49 GMT
WORKDIR /go
# Wed, 13 Jul 2022 07:47:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 07:47:03 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 07:47:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 07:47:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 07:47:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd112bd56ec3e5c889db16588dbcac85cbd1a95bcc45882e8ac837e2315b5c`  
		Last Modified: Wed, 13 Jul 2022 00:12:05 GMT  
		Size: 115.2 MB (115242817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd2cfe75a75aec6138ba0c67d2af1a7a2dd4c5a3b1bde23967b4caef488acb8`  
		Last Modified: Wed, 13 Jul 2022 00:11:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448905a1cc77d184aea8ebe3718f902d023568b6c2f19a1303f82abe51bedd1`  
		Last Modified: Wed, 13 Jul 2022 07:47:36 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996f6eb2c1beceddac26dd5f2c7ad82b7a99fbfbda5afe10a2a07912cedc13f3`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232bb821e1caea148f02346da5fa5562ce283c3cc15a38b5a5075032d51a21`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:703622cb9f18f0b8afa018cad85ee38f07a589dad0efd9a17320f18ecc13cd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122569995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8bede613e41fb58ab47edf7b489bb233d938d4ecdecac92918e083fb05bc964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:16:58 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:21:00 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:21:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:21:02 GMT
WORKDIR /go
# Tue, 12 Jul 2022 22:56:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 12 Jul 2022 22:56:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 00:25:16 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:25:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 00:25:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 00:25:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 00:25:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a482f319cf9a81f236c51c53bb1c689e8b1fa579667d51ca5ed246ee842f0e`  
		Last Modified: Tue, 12 Jul 2022 22:35:48 GMT  
		Size: 111.7 MB (111655243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9920ad3da4e1bfa17727a4264ec8048f45c5117be4799010b8a718e4004cd91`  
		Last Modified: Tue, 12 Jul 2022 22:34:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afe0ff63358ebff72e63d2f0e98d572f7b7705859c43e57f9ef9cfb8447237`  
		Last Modified: Tue, 12 Jul 2022 22:57:30 GMT  
		Size: 6.8 MB (6806683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8e293f9d738d252bf475ce912e8291238915bf42ce57e839482143ab0287d`  
		Last Modified: Wed, 13 Jul 2022 00:26:43 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5f7917a376356834c38ec70309cec40192a27123e32b1516ccdf50a3de64a`  
		Last Modified: Wed, 13 Jul 2022 00:26:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4d18ee072281fc258a9eb19957ead3c8465339eb7b1f5f269afdb3bc9ad4fa09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121402125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6e75b9e1db747dea3dc9c073f2ecaffbce977107e2c900a2163fbdb0297969`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:40 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 01:20:33 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:20:36 GMT
WORKDIR /go
# Thu, 14 Jul 2022 04:51:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Jul 2022 04:51:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 14 Jul 2022 04:51:15 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:51:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Jul 2022 04:51:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Jul 2022 04:51:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Jul 2022 04:51:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e1c3c4b2486777cff8d39eaf101ab399597d87ae5c000dd7b7ad510d46797d`  
		Last Modified: Wed, 13 Jul 2022 01:47:48 GMT  
		Size: 111.4 MB (111423439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309d1e7915b7277aa2caa1a4fdae40f2ca49b928d9fec95e663f3a5711b45e6`  
		Last Modified: Wed, 13 Jul 2022 01:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfb02347c7d72c96558b8bb46a4f048d1e45182f13e10c0e83edf22747ea95`  
		Last Modified: Thu, 14 Jul 2022 04:52:44 GMT  
		Size: 6.1 MB (6067337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e3c4142f91b38c3b1e65fd6fb6ef9628dcc3556482e762152e8c9d1d3c20d`  
		Last Modified: Thu, 14 Jul 2022 04:52:42 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686a634185cb5f4c2d9dba579c1eb3beebb78e69bd25447da60ac8409e08766`  
		Last Modified: Thu, 14 Jul 2022 04:52:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:290cfd704a23c2ddcb1f182f2f17674fdcdbeaeb62282475cfaeb2dcaae9af7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e226abb8bbf011ea45e449c5070530a1ef1cc1df8f81f78ffe8324696cdf73d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:25 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:24:55 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:24:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:24:58 GMT
WORKDIR /go
# Wed, 13 Jul 2022 09:10:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 09:10:54 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 09:10:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 09:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 09:11:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 09:11:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c4cc194face1e292d4841acf35c12d3d21a64fe5cfa594ab6dc52873073ab8`  
		Last Modified: Tue, 12 Jul 2022 22:33:47 GMT  
		Size: 110.3 MB (110292574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685667e0af253c6086e8398208c7561561541b211e9ddbbcf4ef6be883686ef`  
		Last Modified: Tue, 12 Jul 2022 22:33:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db124a84d37b8773dd6f7f3dd17698fb5775f4f372998d4594652b36951c51ed`  
		Last Modified: Wed, 13 Jul 2022 09:11:45 GMT  
		Size: 7.1 MB (7051424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ee509a95002753f22f52015b6d73f187734670231017a28315b2e679616d0`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c79b21287a253cbeff92e71a14c553de9540b34d770e268a8516fa4aa873e8`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:45efd91580c564bafa163224d57cea1742c852d9dbcacc2458d07f2766222c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122018553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe6a5f3afb3907fcc50178a016518559167b721a37de228f9c66eb515bf066f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:04:48 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 05:08:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 05:08:16 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 05:08:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:08:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 05:08:32 GMT
WORKDIR /go
# Wed, 13 Jul 2022 22:11:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 22:11:13 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 22:11:14 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:11:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 22:11:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 22:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 22:11:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a10ac130bb3da5c68d2d1ddd0bddd9c9aafed7a843450be82de6d7afbf936b`  
		Last Modified: Wed, 13 Jul 2022 05:39:52 GMT  
		Size: 110.3 MB (110295902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1b6a1686a88fdc83aa69e21aa8af36292281aded76e23d6478ea562dc6f96`  
		Last Modified: Wed, 13 Jul 2022 05:37:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f614e9e2e974dc8b16c5a51ac52e34a0134a1d53aafdb0b3f5cfa4b5d2856fc`  
		Last Modified: Wed, 13 Jul 2022 22:12:38 GMT  
		Size: 7.5 MB (7481646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94763b8678030186e0f46988e42fc162735c88413e46aaf5ed2a4956f39dd44`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea48a0db2f2ebe6c442a9a51b0febfdd54d1baf5924bc7cb12b54ae2011796d`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7903fc94e9870b09a5c16e5ef6afc2ccb73eb64a00028d57a0a8b954c7d36a3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7170749c53aeec1e443a594cab8e6d8ae65cf4dbd937ab548ffaf95dfefedf94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:35:10 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:37:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 04:38:12 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:38:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:38:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:38:14 GMT
WORKDIR /go
# Wed, 13 Jul 2022 12:23:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 12:23:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 12:23:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:23:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 12:23:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 12:23:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 12:23:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0da7506b596726f522d72670637523b1f1601e15dc1dd4cb1be338164021b`  
		Last Modified: Wed, 13 Jul 2022 04:56:57 GMT  
		Size: 113.2 MB (113165463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78cd6c9206bd154e2ee3a37419413d222f10a31c24af3882cbe40c976c6016`  
		Last Modified: Wed, 13 Jul 2022 04:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15666b0ca68b6455e83f584a5eb1e817b064585023d7a42f80f62a857ae83ec9`  
		Last Modified: Wed, 13 Jul 2022 12:23:56 GMT  
		Size: 7.1 MB (7052809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa673a9dcaa66c8c1003f2b6df47b953e6e58b37233265f1949e78286795d385`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 1.2 MB (1243127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a95a05c45b1aa5d96976995433e8b8a21d81800acaf6535149cdfd51817d5ca`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:343a268d45b94fb60575c5a477f4cf3a62b24e1c1dc6c63a25488c4871c98c69
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
$ docker pull caddy@sha256:2bd3f77e2d21db96ae5a1decdb8df220d98b96e7b812cf7d368828b16bf65ae6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99e5e593f69a4c70d75271117799e5796754e07429560f8f70a6a62a9c09b8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 07:46:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 07:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 07:46:54 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 07:46:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 07:46:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 07:46:58 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 07:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195e97acbd9f5678e292401c0fae3db777aff49e77f38d9cc3f101265b4cdf43`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 291.6 KB (291593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b702741191d81f669709a2af927df34f91029d7bdee74215cf2c65f2270cd`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6330f4d2e50b7bf2126496a3e12ab164af1ad5972222a6dd6ad58fd449b11fe`  
		Last Modified: Wed, 13 Jul 2022 07:47:23 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acec8070f9fa557cb093f66f0b2af0db792a0452918c52d5528fcb4588ad492`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:71bdbcc7ee7d24783e2cf57be294f8c15b313f9c24f41ee4bf4f442c97dc8ba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b22970098c4484f2b4a2c0d563cd0856a595d830bf660a6790517a3e6dc0c04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 00:24:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 00:24:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 00:24:47 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:24:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 00:24:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 00:24:54 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 00:24:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 00:24:59 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 00:24:59 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 00:25:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c75bf2949196f38f164b182514870806879c33b90ec192cdedc33beb7164f3`  
		Last Modified: Wed, 13 Jul 2022 00:26:20 GMT  
		Size: 291.8 KB (291823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e9fed1085fb888faddfae5023a802bb85f365cfde9aacc7b2cf25064c0a7d`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d79f4f39a3e95ed2ada99510758a8816e4ddcf160793887df642ea34d47d6`  
		Last Modified: Wed, 13 Jul 2022 00:26:28 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099d09b43e9c3fdfbe6250cc5340915853372077bf3606d33ba1b9c5bad5c38`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1db5af09e7e93ccc64f39d2aefa6438f3346a62fff17d5f006eef3bf5541424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3d980491df522f57fa63138e24e8c6be022acb10104bab97857a4eab9d04f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 14 Jul 2022 04:50:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 14 Jul 2022 04:50:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 14 Jul 2022 04:50:42 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Jul 2022 04:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 80
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 443
# Thu, 14 Jul 2022 04:50:55 GMT
EXPOSE 2019
# Thu, 14 Jul 2022 04:50:55 GMT
WORKDIR /srv
# Thu, 14 Jul 2022 04:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d2eab8b066328ae05bd108fd3d593cfea00c0c5b4a920788ae29400dfa4fc`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 290.8 KB (290762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e007f0123b4d81f10149eb27d05581180511d1b2884e9f286496e20935f56453`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35e23b17501f974f98785b56b4286fedfcb3e968b0564292daec9ecd9451e`  
		Last Modified: Thu, 14 Jul 2022 04:52:27 GMT  
		Size: 13.3 MB (13347758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbc25b5d1376069d3e359ea4fb05678d63a4a0d20fdce60afc005cfbf344e9`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e277f1e570bb65d07ca7ddaf11bd50b8f64643b579e2a1500165d0d10e873b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15720992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ab296123268f045db4f04fdd9542ea39cf0869b8a5790b52e8359cf4301f2f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 09:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 09:10:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 09:10:27 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 09:10:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 09:10:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 09:10:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 09:10:33 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 09:10:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 09:10:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 09:10:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 09:10:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 09:10:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 09:10:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 09:10:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 09:10:41 GMT
EXPOSE 80
# Wed, 13 Jul 2022 09:10:42 GMT
EXPOSE 443
# Wed, 13 Jul 2022 09:10:43 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 09:10:44 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 09:10:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e2632fbf469bd4459a122146d4f5c544524b9917ebbb1c82ca604c846e6d03`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 291.5 KB (291462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136b5c9b9f23df66b6049078ee2f4df8231ed7eb7f543cc31055c0c338074a3`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d759768dee9c2f0e5c5353760cb5d7fdb641c3bbc7160a9ef0e1428a504a820b`  
		Last Modified: Wed, 13 Jul 2022 09:11:30 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f38216dc74dd3541e3282c41fd26512f9161bbc74eb0fef8374f88c07c33f`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; ppc64le

```console
$ docker pull caddy@sha256:8bf33283df3ab62c0987b87b518be60e587e8e8f492f9001c9f513126218c3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b6dd61b467dc78c47f12742f5af2367935a9ffb8f6dcc8ce8382764c2d1ab8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 22:09:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 22:09:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 22:09:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:10:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 22:10:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 22:10:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 22:10:18 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 22:10:21 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 22:10:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 22:10:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 22:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 22:10:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 22:10:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 22:10:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 22:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 22:10:40 GMT
EXPOSE 80
# Wed, 13 Jul 2022 22:10:43 GMT
EXPOSE 443
# Wed, 13 Jul 2022 22:10:44 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 22:10:48 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 22:10:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49126cc0b1f1c1e51c05b6d7443ed73b5fd2577d177ced4eb36ba827a6b9e68c`  
		Last Modified: Wed, 13 Jul 2022 22:12:19 GMT  
		Size: 293.9 KB (293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f5f92095cf2a8c6afe25b29ea21344778855b89f160fed628effd01704c1c2`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12fbf7d78c1725ab5956092ae9577b979994dc526cbd9f8368c69ce317b692`  
		Last Modified: Wed, 13 Jul 2022 22:12:21 GMT  
		Size: 12.3 MB (12309531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905929de5f23fe3fc6a3b51fc5e5ae5d69bb42d68a20069887fbae365e82fba`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; s390x

```console
$ docker pull caddy@sha256:f3f1634a0c819eb255025ed4f6ed0cf373cf040b4433b99e741b9f356c24f035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db99049e35d90916167a13c53576818e74e4b0f30b57123b9f866b7712c8305b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 12:22:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 12:22:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 12:22:45 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:22:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 12:22:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 12:22:50 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 12:22:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 12:22:53 GMT
EXPOSE 80
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 443
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 12:22:54 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 12:22:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a278a0c4f266219ec8afd82734a3a15f7ad274e786c5e813adde536d23e7a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 291.9 KB (291943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bfcbf66ce9f538fed4132cec8e97597e9ace9340502c5ed98c06909e9369c9`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26380b79ed6fa2324d957b5d5f3c38ae3aaccb280e477850bdae2952a1e1c308`  
		Last Modified: Wed, 13 Jul 2022 12:23:44 GMT  
		Size: 13.5 MB (13460701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319ee79626cacd3ef26113bfb7c3a9086642a88ba734de13a93138ce13b839a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 155.0 B  
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
$ docker pull caddy@sha256:2db1d5975a0e02f6d4ce83d5ff02287989fc3478190a4027aa7c583e0f63e418
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
$ docker pull caddy@sha256:2bd3f77e2d21db96ae5a1decdb8df220d98b96e7b812cf7d368828b16bf65ae6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99e5e593f69a4c70d75271117799e5796754e07429560f8f70a6a62a9c09b8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 07:46:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 07:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 07:46:54 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 07:46:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 07:46:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 07:46:58 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 07:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195e97acbd9f5678e292401c0fae3db777aff49e77f38d9cc3f101265b4cdf43`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 291.6 KB (291593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b702741191d81f669709a2af927df34f91029d7bdee74215cf2c65f2270cd`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6330f4d2e50b7bf2126496a3e12ab164af1ad5972222a6dd6ad58fd449b11fe`  
		Last Modified: Wed, 13 Jul 2022 07:47:23 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acec8070f9fa557cb093f66f0b2af0db792a0452918c52d5528fcb4588ad492`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:71bdbcc7ee7d24783e2cf57be294f8c15b313f9c24f41ee4bf4f442c97dc8ba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b22970098c4484f2b4a2c0d563cd0856a595d830bf660a6790517a3e6dc0c04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 00:24:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 00:24:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 00:24:47 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:24:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 00:24:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 00:24:54 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 00:24:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 00:24:59 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 00:24:59 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 00:25:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c75bf2949196f38f164b182514870806879c33b90ec192cdedc33beb7164f3`  
		Last Modified: Wed, 13 Jul 2022 00:26:20 GMT  
		Size: 291.8 KB (291823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e9fed1085fb888faddfae5023a802bb85f365cfde9aacc7b2cf25064c0a7d`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d79f4f39a3e95ed2ada99510758a8816e4ddcf160793887df642ea34d47d6`  
		Last Modified: Wed, 13 Jul 2022 00:26:28 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099d09b43e9c3fdfbe6250cc5340915853372077bf3606d33ba1b9c5bad5c38`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1db5af09e7e93ccc64f39d2aefa6438f3346a62fff17d5f006eef3bf5541424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3d980491df522f57fa63138e24e8c6be022acb10104bab97857a4eab9d04f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 14 Jul 2022 04:50:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 14 Jul 2022 04:50:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 14 Jul 2022 04:50:42 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Jul 2022 04:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 80
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 443
# Thu, 14 Jul 2022 04:50:55 GMT
EXPOSE 2019
# Thu, 14 Jul 2022 04:50:55 GMT
WORKDIR /srv
# Thu, 14 Jul 2022 04:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d2eab8b066328ae05bd108fd3d593cfea00c0c5b4a920788ae29400dfa4fc`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 290.8 KB (290762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e007f0123b4d81f10149eb27d05581180511d1b2884e9f286496e20935f56453`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35e23b17501f974f98785b56b4286fedfcb3e968b0564292daec9ecd9451e`  
		Last Modified: Thu, 14 Jul 2022 04:52:27 GMT  
		Size: 13.3 MB (13347758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbc25b5d1376069d3e359ea4fb05678d63a4a0d20fdce60afc005cfbf344e9`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e277f1e570bb65d07ca7ddaf11bd50b8f64643b579e2a1500165d0d10e873b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15720992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ab296123268f045db4f04fdd9542ea39cf0869b8a5790b52e8359cf4301f2f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 09:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 09:10:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 09:10:27 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 09:10:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 09:10:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 09:10:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 09:10:33 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 09:10:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 09:10:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 09:10:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 09:10:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 09:10:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 09:10:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 09:10:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 09:10:41 GMT
EXPOSE 80
# Wed, 13 Jul 2022 09:10:42 GMT
EXPOSE 443
# Wed, 13 Jul 2022 09:10:43 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 09:10:44 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 09:10:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e2632fbf469bd4459a122146d4f5c544524b9917ebbb1c82ca604c846e6d03`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 291.5 KB (291462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136b5c9b9f23df66b6049078ee2f4df8231ed7eb7f543cc31055c0c338074a3`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d759768dee9c2f0e5c5353760cb5d7fdb641c3bbc7160a9ef0e1428a504a820b`  
		Last Modified: Wed, 13 Jul 2022 09:11:30 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f38216dc74dd3541e3282c41fd26512f9161bbc74eb0fef8374f88c07c33f`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8bf33283df3ab62c0987b87b518be60e587e8e8f492f9001c9f513126218c3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b6dd61b467dc78c47f12742f5af2367935a9ffb8f6dcc8ce8382764c2d1ab8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 22:09:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 22:09:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 22:09:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:10:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 22:10:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 22:10:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 22:10:18 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 22:10:21 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 22:10:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 22:10:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 22:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 22:10:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 22:10:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 22:10:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 22:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 22:10:40 GMT
EXPOSE 80
# Wed, 13 Jul 2022 22:10:43 GMT
EXPOSE 443
# Wed, 13 Jul 2022 22:10:44 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 22:10:48 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 22:10:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49126cc0b1f1c1e51c05b6d7443ed73b5fd2577d177ced4eb36ba827a6b9e68c`  
		Last Modified: Wed, 13 Jul 2022 22:12:19 GMT  
		Size: 293.9 KB (293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f5f92095cf2a8c6afe25b29ea21344778855b89f160fed628effd01704c1c2`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12fbf7d78c1725ab5956092ae9577b979994dc526cbd9f8368c69ce317b692`  
		Last Modified: Wed, 13 Jul 2022 22:12:21 GMT  
		Size: 12.3 MB (12309531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905929de5f23fe3fc6a3b51fc5e5ae5d69bb42d68a20069887fbae365e82fba`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f3f1634a0c819eb255025ed4f6ed0cf373cf040b4433b99e741b9f356c24f035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db99049e35d90916167a13c53576818e74e4b0f30b57123b9f866b7712c8305b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 12:22:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 12:22:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 12:22:45 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:22:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 12:22:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 12:22:50 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 12:22:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 12:22:53 GMT
EXPOSE 80
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 443
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 12:22:54 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 12:22:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a278a0c4f266219ec8afd82734a3a15f7ad274e786c5e813adde536d23e7a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 291.9 KB (291943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bfcbf66ce9f538fed4132cec8e97597e9ace9340502c5ed98c06909e9369c9`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26380b79ed6fa2324d957b5d5f3c38ae3aaccb280e477850bdae2952a1e1c308`  
		Last Modified: Wed, 13 Jul 2022 12:23:44 GMT  
		Size: 13.5 MB (13460701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319ee79626cacd3ef26113bfb7c3a9086642a88ba734de13a93138ce13b839a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder`

```console
$ docker pull caddy@sha256:f68592219340bb743bb752f7c4c5711a95693066900a45c88ef1a99fd59f7a99
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
$ docker pull caddy@sha256:83d4d0707f0fdf954311174224be106071959f6cadb80a90349f481eae9fb2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126544689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a1b98417a84b3a24a165471d7d84c070cc923dac2d4c9d1f893e347b24d418`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:12 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:01:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 00:01:48 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:01:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:01:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:01:49 GMT
WORKDIR /go
# Wed, 13 Jul 2022 07:47:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 07:47:03 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 07:47:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 07:47:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 07:47:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd112bd56ec3e5c889db16588dbcac85cbd1a95bcc45882e8ac837e2315b5c`  
		Last Modified: Wed, 13 Jul 2022 00:12:05 GMT  
		Size: 115.2 MB (115242817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd2cfe75a75aec6138ba0c67d2af1a7a2dd4c5a3b1bde23967b4caef488acb8`  
		Last Modified: Wed, 13 Jul 2022 00:11:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448905a1cc77d184aea8ebe3718f902d023568b6c2f19a1303f82abe51bedd1`  
		Last Modified: Wed, 13 Jul 2022 07:47:36 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996f6eb2c1beceddac26dd5f2c7ad82b7a99fbfbda5afe10a2a07912cedc13f3`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232bb821e1caea148f02346da5fa5562ce283c3cc15a38b5a5075032d51a21`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:703622cb9f18f0b8afa018cad85ee38f07a589dad0efd9a17320f18ecc13cd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122569995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8bede613e41fb58ab47edf7b489bb233d938d4ecdecac92918e083fb05bc964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:16:58 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:21:00 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:21:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:21:02 GMT
WORKDIR /go
# Tue, 12 Jul 2022 22:56:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 12 Jul 2022 22:56:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 00:25:16 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:25:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 00:25:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 00:25:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 00:25:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a482f319cf9a81f236c51c53bb1c689e8b1fa579667d51ca5ed246ee842f0e`  
		Last Modified: Tue, 12 Jul 2022 22:35:48 GMT  
		Size: 111.7 MB (111655243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9920ad3da4e1bfa17727a4264ec8048f45c5117be4799010b8a718e4004cd91`  
		Last Modified: Tue, 12 Jul 2022 22:34:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afe0ff63358ebff72e63d2f0e98d572f7b7705859c43e57f9ef9cfb8447237`  
		Last Modified: Tue, 12 Jul 2022 22:57:30 GMT  
		Size: 6.8 MB (6806683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8e293f9d738d252bf475ce912e8291238915bf42ce57e839482143ab0287d`  
		Last Modified: Wed, 13 Jul 2022 00:26:43 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5f7917a376356834c38ec70309cec40192a27123e32b1516ccdf50a3de64a`  
		Last Modified: Wed, 13 Jul 2022 00:26:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4d18ee072281fc258a9eb19957ead3c8465339eb7b1f5f269afdb3bc9ad4fa09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121402125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6e75b9e1db747dea3dc9c073f2ecaffbce977107e2c900a2163fbdb0297969`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:40 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 01:20:33 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:20:36 GMT
WORKDIR /go
# Thu, 14 Jul 2022 04:51:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Jul 2022 04:51:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 14 Jul 2022 04:51:15 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:51:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Jul 2022 04:51:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Jul 2022 04:51:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Jul 2022 04:51:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e1c3c4b2486777cff8d39eaf101ab399597d87ae5c000dd7b7ad510d46797d`  
		Last Modified: Wed, 13 Jul 2022 01:47:48 GMT  
		Size: 111.4 MB (111423439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309d1e7915b7277aa2caa1a4fdae40f2ca49b928d9fec95e663f3a5711b45e6`  
		Last Modified: Wed, 13 Jul 2022 01:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfb02347c7d72c96558b8bb46a4f048d1e45182f13e10c0e83edf22747ea95`  
		Last Modified: Thu, 14 Jul 2022 04:52:44 GMT  
		Size: 6.1 MB (6067337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e3c4142f91b38c3b1e65fd6fb6ef9628dcc3556482e762152e8c9d1d3c20d`  
		Last Modified: Thu, 14 Jul 2022 04:52:42 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686a634185cb5f4c2d9dba579c1eb3beebb78e69bd25447da60ac8409e08766`  
		Last Modified: Thu, 14 Jul 2022 04:52:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:290cfd704a23c2ddcb1f182f2f17674fdcdbeaeb62282475cfaeb2dcaae9af7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e226abb8bbf011ea45e449c5070530a1ef1cc1df8f81f78ffe8324696cdf73d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:25 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:24:55 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:24:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:24:58 GMT
WORKDIR /go
# Wed, 13 Jul 2022 09:10:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 09:10:54 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 09:10:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 09:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 09:11:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 09:11:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c4cc194face1e292d4841acf35c12d3d21a64fe5cfa594ab6dc52873073ab8`  
		Last Modified: Tue, 12 Jul 2022 22:33:47 GMT  
		Size: 110.3 MB (110292574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685667e0af253c6086e8398208c7561561541b211e9ddbbcf4ef6be883686ef`  
		Last Modified: Tue, 12 Jul 2022 22:33:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db124a84d37b8773dd6f7f3dd17698fb5775f4f372998d4594652b36951c51ed`  
		Last Modified: Wed, 13 Jul 2022 09:11:45 GMT  
		Size: 7.1 MB (7051424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ee509a95002753f22f52015b6d73f187734670231017a28315b2e679616d0`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c79b21287a253cbeff92e71a14c553de9540b34d770e268a8516fa4aa873e8`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:45efd91580c564bafa163224d57cea1742c852d9dbcacc2458d07f2766222c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122018553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe6a5f3afb3907fcc50178a016518559167b721a37de228f9c66eb515bf066f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:04:48 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 05:08:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 05:08:16 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 05:08:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:08:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 05:08:32 GMT
WORKDIR /go
# Wed, 13 Jul 2022 22:11:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 22:11:13 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 22:11:14 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:11:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 22:11:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 22:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 22:11:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a10ac130bb3da5c68d2d1ddd0bddd9c9aafed7a843450be82de6d7afbf936b`  
		Last Modified: Wed, 13 Jul 2022 05:39:52 GMT  
		Size: 110.3 MB (110295902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1b6a1686a88fdc83aa69e21aa8af36292281aded76e23d6478ea562dc6f96`  
		Last Modified: Wed, 13 Jul 2022 05:37:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f614e9e2e974dc8b16c5a51ac52e34a0134a1d53aafdb0b3f5cfa4b5d2856fc`  
		Last Modified: Wed, 13 Jul 2022 22:12:38 GMT  
		Size: 7.5 MB (7481646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94763b8678030186e0f46988e42fc162735c88413e46aaf5ed2a4956f39dd44`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea48a0db2f2ebe6c442a9a51b0febfdd54d1baf5924bc7cb12b54ae2011796d`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7903fc94e9870b09a5c16e5ef6afc2ccb73eb64a00028d57a0a8b954c7d36a3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7170749c53aeec1e443a594cab8e6d8ae65cf4dbd937ab548ffaf95dfefedf94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:35:10 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:37:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 04:38:12 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:38:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:38:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:38:14 GMT
WORKDIR /go
# Wed, 13 Jul 2022 12:23:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 12:23:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 12:23:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:23:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 12:23:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 12:23:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 12:23:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0da7506b596726f522d72670637523b1f1601e15dc1dd4cb1be338164021b`  
		Last Modified: Wed, 13 Jul 2022 04:56:57 GMT  
		Size: 113.2 MB (113165463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78cd6c9206bd154e2ee3a37419413d222f10a31c24af3882cbe40c976c6016`  
		Last Modified: Wed, 13 Jul 2022 04:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15666b0ca68b6455e83f584a5eb1e817b064585023d7a42f80f62a857ae83ec9`  
		Last Modified: Wed, 13 Jul 2022 12:23:56 GMT  
		Size: 7.1 MB (7052809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa673a9dcaa66c8c1003f2b6df47b953e6e58b37233265f1949e78286795d385`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 1.2 MB (1243127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a95a05c45b1aa5d96976995433e8b8a21d81800acaf6535149cdfd51817d5ca`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:e6697d7888f6b3af8a07ad6f89ba4f7a556aad9b22e17a36fbc9d57146b82a99
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
$ docker pull caddy@sha256:83d4d0707f0fdf954311174224be106071959f6cadb80a90349f481eae9fb2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126544689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a1b98417a84b3a24a165471d7d84c070cc923dac2d4c9d1f893e347b24d418`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:12 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:01:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 00:01:48 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:01:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:01:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:01:49 GMT
WORKDIR /go
# Wed, 13 Jul 2022 07:47:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 07:47:03 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 07:47:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 07:47:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 07:47:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd112bd56ec3e5c889db16588dbcac85cbd1a95bcc45882e8ac837e2315b5c`  
		Last Modified: Wed, 13 Jul 2022 00:12:05 GMT  
		Size: 115.2 MB (115242817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd2cfe75a75aec6138ba0c67d2af1a7a2dd4c5a3b1bde23967b4caef488acb8`  
		Last Modified: Wed, 13 Jul 2022 00:11:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448905a1cc77d184aea8ebe3718f902d023568b6c2f19a1303f82abe51bedd1`  
		Last Modified: Wed, 13 Jul 2022 07:47:36 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996f6eb2c1beceddac26dd5f2c7ad82b7a99fbfbda5afe10a2a07912cedc13f3`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232bb821e1caea148f02346da5fa5562ce283c3cc15a38b5a5075032d51a21`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:703622cb9f18f0b8afa018cad85ee38f07a589dad0efd9a17320f18ecc13cd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122569995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8bede613e41fb58ab47edf7b489bb233d938d4ecdecac92918e083fb05bc964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:16:58 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:21:00 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:21:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:21:02 GMT
WORKDIR /go
# Tue, 12 Jul 2022 22:56:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 12 Jul 2022 22:56:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 00:25:16 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:25:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 00:25:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 00:25:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 00:25:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a482f319cf9a81f236c51c53bb1c689e8b1fa579667d51ca5ed246ee842f0e`  
		Last Modified: Tue, 12 Jul 2022 22:35:48 GMT  
		Size: 111.7 MB (111655243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9920ad3da4e1bfa17727a4264ec8048f45c5117be4799010b8a718e4004cd91`  
		Last Modified: Tue, 12 Jul 2022 22:34:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afe0ff63358ebff72e63d2f0e98d572f7b7705859c43e57f9ef9cfb8447237`  
		Last Modified: Tue, 12 Jul 2022 22:57:30 GMT  
		Size: 6.8 MB (6806683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8e293f9d738d252bf475ce912e8291238915bf42ce57e839482143ab0287d`  
		Last Modified: Wed, 13 Jul 2022 00:26:43 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5f7917a376356834c38ec70309cec40192a27123e32b1516ccdf50a3de64a`  
		Last Modified: Wed, 13 Jul 2022 00:26:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4d18ee072281fc258a9eb19957ead3c8465339eb7b1f5f269afdb3bc9ad4fa09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121402125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6e75b9e1db747dea3dc9c073f2ecaffbce977107e2c900a2163fbdb0297969`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:40 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 01:20:33 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:20:36 GMT
WORKDIR /go
# Thu, 14 Jul 2022 04:51:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Jul 2022 04:51:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 14 Jul 2022 04:51:15 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:51:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Jul 2022 04:51:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Jul 2022 04:51:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Jul 2022 04:51:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e1c3c4b2486777cff8d39eaf101ab399597d87ae5c000dd7b7ad510d46797d`  
		Last Modified: Wed, 13 Jul 2022 01:47:48 GMT  
		Size: 111.4 MB (111423439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309d1e7915b7277aa2caa1a4fdae40f2ca49b928d9fec95e663f3a5711b45e6`  
		Last Modified: Wed, 13 Jul 2022 01:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfb02347c7d72c96558b8bb46a4f048d1e45182f13e10c0e83edf22747ea95`  
		Last Modified: Thu, 14 Jul 2022 04:52:44 GMT  
		Size: 6.1 MB (6067337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e3c4142f91b38c3b1e65fd6fb6ef9628dcc3556482e762152e8c9d1d3c20d`  
		Last Modified: Thu, 14 Jul 2022 04:52:42 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686a634185cb5f4c2d9dba579c1eb3beebb78e69bd25447da60ac8409e08766`  
		Last Modified: Thu, 14 Jul 2022 04:52:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:290cfd704a23c2ddcb1f182f2f17674fdcdbeaeb62282475cfaeb2dcaae9af7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e226abb8bbf011ea45e449c5070530a1ef1cc1df8f81f78ffe8324696cdf73d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:25 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:24:55 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:24:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:24:58 GMT
WORKDIR /go
# Wed, 13 Jul 2022 09:10:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 09:10:54 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 09:10:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 09:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 09:11:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 09:11:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c4cc194face1e292d4841acf35c12d3d21a64fe5cfa594ab6dc52873073ab8`  
		Last Modified: Tue, 12 Jul 2022 22:33:47 GMT  
		Size: 110.3 MB (110292574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685667e0af253c6086e8398208c7561561541b211e9ddbbcf4ef6be883686ef`  
		Last Modified: Tue, 12 Jul 2022 22:33:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db124a84d37b8773dd6f7f3dd17698fb5775f4f372998d4594652b36951c51ed`  
		Last Modified: Wed, 13 Jul 2022 09:11:45 GMT  
		Size: 7.1 MB (7051424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ee509a95002753f22f52015b6d73f187734670231017a28315b2e679616d0`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c79b21287a253cbeff92e71a14c553de9540b34d770e268a8516fa4aa873e8`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:45efd91580c564bafa163224d57cea1742c852d9dbcacc2458d07f2766222c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122018553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe6a5f3afb3907fcc50178a016518559167b721a37de228f9c66eb515bf066f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:04:48 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 05:08:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 05:08:16 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 05:08:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:08:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 05:08:32 GMT
WORKDIR /go
# Wed, 13 Jul 2022 22:11:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 22:11:13 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 22:11:14 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:11:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 22:11:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 22:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 22:11:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a10ac130bb3da5c68d2d1ddd0bddd9c9aafed7a843450be82de6d7afbf936b`  
		Last Modified: Wed, 13 Jul 2022 05:39:52 GMT  
		Size: 110.3 MB (110295902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1b6a1686a88fdc83aa69e21aa8af36292281aded76e23d6478ea562dc6f96`  
		Last Modified: Wed, 13 Jul 2022 05:37:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f614e9e2e974dc8b16c5a51ac52e34a0134a1d53aafdb0b3f5cfa4b5d2856fc`  
		Last Modified: Wed, 13 Jul 2022 22:12:38 GMT  
		Size: 7.5 MB (7481646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94763b8678030186e0f46988e42fc162735c88413e46aaf5ed2a4956f39dd44`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea48a0db2f2ebe6c442a9a51b0febfdd54d1baf5924bc7cb12b54ae2011796d`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7903fc94e9870b09a5c16e5ef6afc2ccb73eb64a00028d57a0a8b954c7d36a3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7170749c53aeec1e443a594cab8e6d8ae65cf4dbd937ab548ffaf95dfefedf94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:35:10 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:37:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 04:38:12 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:38:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:38:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:38:14 GMT
WORKDIR /go
# Wed, 13 Jul 2022 12:23:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 12:23:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 12:23:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:23:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 12:23:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 12:23:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 12:23:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0da7506b596726f522d72670637523b1f1601e15dc1dd4cb1be338164021b`  
		Last Modified: Wed, 13 Jul 2022 04:56:57 GMT  
		Size: 113.2 MB (113165463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78cd6c9206bd154e2ee3a37419413d222f10a31c24af3882cbe40c976c6016`  
		Last Modified: Wed, 13 Jul 2022 04:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15666b0ca68b6455e83f584a5eb1e817b064585023d7a42f80f62a857ae83ec9`  
		Last Modified: Wed, 13 Jul 2022 12:23:56 GMT  
		Size: 7.1 MB (7052809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa673a9dcaa66c8c1003f2b6df47b953e6e58b37233265f1949e78286795d385`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 1.2 MB (1243127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a95a05c45b1aa5d96976995433e8b8a21d81800acaf6535149cdfd51817d5ca`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:2db1d5975a0e02f6d4ce83d5ff02287989fc3478190a4027aa7c583e0f63e418
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
$ docker pull caddy@sha256:2bd3f77e2d21db96ae5a1decdb8df220d98b96e7b812cf7d368828b16bf65ae6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99e5e593f69a4c70d75271117799e5796754e07429560f8f70a6a62a9c09b8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 07:46:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 07:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 07:46:54 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 07:46:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 07:46:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 07:46:58 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 07:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195e97acbd9f5678e292401c0fae3db777aff49e77f38d9cc3f101265b4cdf43`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 291.6 KB (291593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b702741191d81f669709a2af927df34f91029d7bdee74215cf2c65f2270cd`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6330f4d2e50b7bf2126496a3e12ab164af1ad5972222a6dd6ad58fd449b11fe`  
		Last Modified: Wed, 13 Jul 2022 07:47:23 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acec8070f9fa557cb093f66f0b2af0db792a0452918c52d5528fcb4588ad492`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:71bdbcc7ee7d24783e2cf57be294f8c15b313f9c24f41ee4bf4f442c97dc8ba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b22970098c4484f2b4a2c0d563cd0856a595d830bf660a6790517a3e6dc0c04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 00:24:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 00:24:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 00:24:47 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:24:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 00:24:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 00:24:54 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 00:24:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 00:24:59 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 00:24:59 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 00:25:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c75bf2949196f38f164b182514870806879c33b90ec192cdedc33beb7164f3`  
		Last Modified: Wed, 13 Jul 2022 00:26:20 GMT  
		Size: 291.8 KB (291823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e9fed1085fb888faddfae5023a802bb85f365cfde9aacc7b2cf25064c0a7d`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d79f4f39a3e95ed2ada99510758a8816e4ddcf160793887df642ea34d47d6`  
		Last Modified: Wed, 13 Jul 2022 00:26:28 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099d09b43e9c3fdfbe6250cc5340915853372077bf3606d33ba1b9c5bad5c38`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1db5af09e7e93ccc64f39d2aefa6438f3346a62fff17d5f006eef3bf5541424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3d980491df522f57fa63138e24e8c6be022acb10104bab97857a4eab9d04f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 14 Jul 2022 04:50:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 14 Jul 2022 04:50:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 14 Jul 2022 04:50:42 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Jul 2022 04:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 80
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 443
# Thu, 14 Jul 2022 04:50:55 GMT
EXPOSE 2019
# Thu, 14 Jul 2022 04:50:55 GMT
WORKDIR /srv
# Thu, 14 Jul 2022 04:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d2eab8b066328ae05bd108fd3d593cfea00c0c5b4a920788ae29400dfa4fc`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 290.8 KB (290762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e007f0123b4d81f10149eb27d05581180511d1b2884e9f286496e20935f56453`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35e23b17501f974f98785b56b4286fedfcb3e968b0564292daec9ecd9451e`  
		Last Modified: Thu, 14 Jul 2022 04:52:27 GMT  
		Size: 13.3 MB (13347758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbc25b5d1376069d3e359ea4fb05678d63a4a0d20fdce60afc005cfbf344e9`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e277f1e570bb65d07ca7ddaf11bd50b8f64643b579e2a1500165d0d10e873b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15720992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ab296123268f045db4f04fdd9542ea39cf0869b8a5790b52e8359cf4301f2f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 09:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 09:10:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 09:10:27 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 09:10:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 09:10:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 09:10:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 09:10:33 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 09:10:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 09:10:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 09:10:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 09:10:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 09:10:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 09:10:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 09:10:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 09:10:41 GMT
EXPOSE 80
# Wed, 13 Jul 2022 09:10:42 GMT
EXPOSE 443
# Wed, 13 Jul 2022 09:10:43 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 09:10:44 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 09:10:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e2632fbf469bd4459a122146d4f5c544524b9917ebbb1c82ca604c846e6d03`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 291.5 KB (291462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136b5c9b9f23df66b6049078ee2f4df8231ed7eb7f543cc31055c0c338074a3`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d759768dee9c2f0e5c5353760cb5d7fdb641c3bbc7160a9ef0e1428a504a820b`  
		Last Modified: Wed, 13 Jul 2022 09:11:30 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f38216dc74dd3541e3282c41fd26512f9161bbc74eb0fef8374f88c07c33f`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8bf33283df3ab62c0987b87b518be60e587e8e8f492f9001c9f513126218c3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b6dd61b467dc78c47f12742f5af2367935a9ffb8f6dcc8ce8382764c2d1ab8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 22:09:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 22:09:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 22:09:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:10:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 22:10:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 22:10:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 22:10:18 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 22:10:21 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 22:10:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 22:10:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 22:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 22:10:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 22:10:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 22:10:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 22:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 22:10:40 GMT
EXPOSE 80
# Wed, 13 Jul 2022 22:10:43 GMT
EXPOSE 443
# Wed, 13 Jul 2022 22:10:44 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 22:10:48 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 22:10:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49126cc0b1f1c1e51c05b6d7443ed73b5fd2577d177ced4eb36ba827a6b9e68c`  
		Last Modified: Wed, 13 Jul 2022 22:12:19 GMT  
		Size: 293.9 KB (293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f5f92095cf2a8c6afe25b29ea21344778855b89f160fed628effd01704c1c2`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12fbf7d78c1725ab5956092ae9577b979994dc526cbd9f8368c69ce317b692`  
		Last Modified: Wed, 13 Jul 2022 22:12:21 GMT  
		Size: 12.3 MB (12309531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905929de5f23fe3fc6a3b51fc5e5ae5d69bb42d68a20069887fbae365e82fba`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f3f1634a0c819eb255025ed4f6ed0cf373cf040b4433b99e741b9f356c24f035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db99049e35d90916167a13c53576818e74e4b0f30b57123b9f866b7712c8305b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 12:22:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 12:22:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 12:22:45 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:22:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 12:22:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 12:22:50 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 12:22:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 12:22:53 GMT
EXPOSE 80
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 443
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 12:22:54 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 12:22:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a278a0c4f266219ec8afd82734a3a15f7ad274e786c5e813adde536d23e7a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 291.9 KB (291943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bfcbf66ce9f538fed4132cec8e97597e9ace9340502c5ed98c06909e9369c9`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26380b79ed6fa2324d957b5d5f3c38ae3aaccb280e477850bdae2952a1e1c308`  
		Last Modified: Wed, 13 Jul 2022 12:23:44 GMT  
		Size: 13.5 MB (13460701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319ee79626cacd3ef26113bfb7c3a9086642a88ba734de13a93138ce13b839a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:f68592219340bb743bb752f7c4c5711a95693066900a45c88ef1a99fd59f7a99
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
$ docker pull caddy@sha256:83d4d0707f0fdf954311174224be106071959f6cadb80a90349f481eae9fb2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126544689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a1b98417a84b3a24a165471d7d84c070cc923dac2d4c9d1f893e347b24d418`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:12 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:01:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 00:01:48 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:01:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:01:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:01:49 GMT
WORKDIR /go
# Wed, 13 Jul 2022 07:47:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 07:47:03 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 07:47:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 07:47:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 07:47:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd112bd56ec3e5c889db16588dbcac85cbd1a95bcc45882e8ac837e2315b5c`  
		Last Modified: Wed, 13 Jul 2022 00:12:05 GMT  
		Size: 115.2 MB (115242817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd2cfe75a75aec6138ba0c67d2af1a7a2dd4c5a3b1bde23967b4caef488acb8`  
		Last Modified: Wed, 13 Jul 2022 00:11:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448905a1cc77d184aea8ebe3718f902d023568b6c2f19a1303f82abe51bedd1`  
		Last Modified: Wed, 13 Jul 2022 07:47:36 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996f6eb2c1beceddac26dd5f2c7ad82b7a99fbfbda5afe10a2a07912cedc13f3`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232bb821e1caea148f02346da5fa5562ce283c3cc15a38b5a5075032d51a21`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:703622cb9f18f0b8afa018cad85ee38f07a589dad0efd9a17320f18ecc13cd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122569995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8bede613e41fb58ab47edf7b489bb233d938d4ecdecac92918e083fb05bc964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:16:58 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:21:00 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:21:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:21:02 GMT
WORKDIR /go
# Tue, 12 Jul 2022 22:56:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 12 Jul 2022 22:56:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 00:25:16 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:25:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 00:25:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 00:25:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 00:25:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a482f319cf9a81f236c51c53bb1c689e8b1fa579667d51ca5ed246ee842f0e`  
		Last Modified: Tue, 12 Jul 2022 22:35:48 GMT  
		Size: 111.7 MB (111655243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9920ad3da4e1bfa17727a4264ec8048f45c5117be4799010b8a718e4004cd91`  
		Last Modified: Tue, 12 Jul 2022 22:34:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afe0ff63358ebff72e63d2f0e98d572f7b7705859c43e57f9ef9cfb8447237`  
		Last Modified: Tue, 12 Jul 2022 22:57:30 GMT  
		Size: 6.8 MB (6806683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8e293f9d738d252bf475ce912e8291238915bf42ce57e839482143ab0287d`  
		Last Modified: Wed, 13 Jul 2022 00:26:43 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5f7917a376356834c38ec70309cec40192a27123e32b1516ccdf50a3de64a`  
		Last Modified: Wed, 13 Jul 2022 00:26:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4d18ee072281fc258a9eb19957ead3c8465339eb7b1f5f269afdb3bc9ad4fa09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121402125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6e75b9e1db747dea3dc9c073f2ecaffbce977107e2c900a2163fbdb0297969`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:40 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 01:20:33 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:20:36 GMT
WORKDIR /go
# Thu, 14 Jul 2022 04:51:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Jul 2022 04:51:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 14 Jul 2022 04:51:15 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:51:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Jul 2022 04:51:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Jul 2022 04:51:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Jul 2022 04:51:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e1c3c4b2486777cff8d39eaf101ab399597d87ae5c000dd7b7ad510d46797d`  
		Last Modified: Wed, 13 Jul 2022 01:47:48 GMT  
		Size: 111.4 MB (111423439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309d1e7915b7277aa2caa1a4fdae40f2ca49b928d9fec95e663f3a5711b45e6`  
		Last Modified: Wed, 13 Jul 2022 01:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfb02347c7d72c96558b8bb46a4f048d1e45182f13e10c0e83edf22747ea95`  
		Last Modified: Thu, 14 Jul 2022 04:52:44 GMT  
		Size: 6.1 MB (6067337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e3c4142f91b38c3b1e65fd6fb6ef9628dcc3556482e762152e8c9d1d3c20d`  
		Last Modified: Thu, 14 Jul 2022 04:52:42 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686a634185cb5f4c2d9dba579c1eb3beebb78e69bd25447da60ac8409e08766`  
		Last Modified: Thu, 14 Jul 2022 04:52:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:290cfd704a23c2ddcb1f182f2f17674fdcdbeaeb62282475cfaeb2dcaae9af7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e226abb8bbf011ea45e449c5070530a1ef1cc1df8f81f78ffe8324696cdf73d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:25 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:24:55 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:24:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:24:58 GMT
WORKDIR /go
# Wed, 13 Jul 2022 09:10:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 09:10:54 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 09:10:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 09:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 09:11:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 09:11:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c4cc194face1e292d4841acf35c12d3d21a64fe5cfa594ab6dc52873073ab8`  
		Last Modified: Tue, 12 Jul 2022 22:33:47 GMT  
		Size: 110.3 MB (110292574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685667e0af253c6086e8398208c7561561541b211e9ddbbcf4ef6be883686ef`  
		Last Modified: Tue, 12 Jul 2022 22:33:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db124a84d37b8773dd6f7f3dd17698fb5775f4f372998d4594652b36951c51ed`  
		Last Modified: Wed, 13 Jul 2022 09:11:45 GMT  
		Size: 7.1 MB (7051424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ee509a95002753f22f52015b6d73f187734670231017a28315b2e679616d0`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c79b21287a253cbeff92e71a14c553de9540b34d770e268a8516fa4aa873e8`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:45efd91580c564bafa163224d57cea1742c852d9dbcacc2458d07f2766222c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122018553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe6a5f3afb3907fcc50178a016518559167b721a37de228f9c66eb515bf066f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:04:48 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 05:08:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 05:08:16 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 05:08:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:08:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 05:08:32 GMT
WORKDIR /go
# Wed, 13 Jul 2022 22:11:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 22:11:13 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 22:11:14 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:11:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 22:11:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 22:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 22:11:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a10ac130bb3da5c68d2d1ddd0bddd9c9aafed7a843450be82de6d7afbf936b`  
		Last Modified: Wed, 13 Jul 2022 05:39:52 GMT  
		Size: 110.3 MB (110295902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1b6a1686a88fdc83aa69e21aa8af36292281aded76e23d6478ea562dc6f96`  
		Last Modified: Wed, 13 Jul 2022 05:37:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f614e9e2e974dc8b16c5a51ac52e34a0134a1d53aafdb0b3f5cfa4b5d2856fc`  
		Last Modified: Wed, 13 Jul 2022 22:12:38 GMT  
		Size: 7.5 MB (7481646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94763b8678030186e0f46988e42fc162735c88413e46aaf5ed2a4956f39dd44`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea48a0db2f2ebe6c442a9a51b0febfdd54d1baf5924bc7cb12b54ae2011796d`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:7903fc94e9870b09a5c16e5ef6afc2ccb73eb64a00028d57a0a8b954c7d36a3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7170749c53aeec1e443a594cab8e6d8ae65cf4dbd937ab548ffaf95dfefedf94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:35:10 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:37:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 04:38:12 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:38:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:38:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:38:14 GMT
WORKDIR /go
# Wed, 13 Jul 2022 12:23:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 12:23:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 12:23:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:23:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 12:23:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 12:23:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 12:23:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0da7506b596726f522d72670637523b1f1601e15dc1dd4cb1be338164021b`  
		Last Modified: Wed, 13 Jul 2022 04:56:57 GMT  
		Size: 113.2 MB (113165463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78cd6c9206bd154e2ee3a37419413d222f10a31c24af3882cbe40c976c6016`  
		Last Modified: Wed, 13 Jul 2022 04:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15666b0ca68b6455e83f584a5eb1e817b064585023d7a42f80f62a857ae83ec9`  
		Last Modified: Wed, 13 Jul 2022 12:23:56 GMT  
		Size: 7.1 MB (7052809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa673a9dcaa66c8c1003f2b6df47b953e6e58b37233265f1949e78286795d385`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 1.2 MB (1243127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a95a05c45b1aa5d96976995433e8b8a21d81800acaf6535149cdfd51817d5ca`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:e6697d7888f6b3af8a07ad6f89ba4f7a556aad9b22e17a36fbc9d57146b82a99
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
$ docker pull caddy@sha256:83d4d0707f0fdf954311174224be106071959f6cadb80a90349f481eae9fb2a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126544689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a1b98417a84b3a24a165471d7d84c070cc923dac2d4c9d1f893e347b24d418`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:19:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:19:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:12 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:01:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 00:01:48 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:01:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:01:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:01:49 GMT
WORKDIR /go
# Wed, 13 Jul 2022 07:47:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 07:47:03 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 07:47:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 07:47:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 07:47:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60b727a1ce729d031ec1e4f2521a246e71bdb72d3fd9c9c04711cce80e1722`  
		Last Modified: Wed, 25 May 2022 00:24:05 GMT  
		Size: 271.8 KB (271822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c4a77219572e69864cd3069b7b47e55202681be151bd7394f9cb6645b5687b`  
		Last Modified: Wed, 25 May 2022 00:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd112bd56ec3e5c889db16588dbcac85cbd1a95bcc45882e8ac837e2315b5c`  
		Last Modified: Wed, 13 Jul 2022 00:12:05 GMT  
		Size: 115.2 MB (115242817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd2cfe75a75aec6138ba0c67d2af1a7a2dd4c5a3b1bde23967b4caef488acb8`  
		Last Modified: Wed, 13 Jul 2022 00:11:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448905a1cc77d184aea8ebe3718f902d023568b6c2f19a1303f82abe51bedd1`  
		Last Modified: Wed, 13 Jul 2022 07:47:36 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996f6eb2c1beceddac26dd5f2c7ad82b7a99fbfbda5afe10a2a07912cedc13f3`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232bb821e1caea148f02346da5fa5562ce283c3cc15a38b5a5075032d51a21`  
		Last Modified: Wed, 13 Jul 2022 07:47:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:703622cb9f18f0b8afa018cad85ee38f07a589dad0efd9a17320f18ecc13cd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122569995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8bede613e41fb58ab47edf7b489bb233d938d4ecdecac92918e083fb05bc964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:49:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:49:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:16:58 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:21:00 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:21:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:21:02 GMT
WORKDIR /go
# Tue, 12 Jul 2022 22:56:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 12 Jul 2022 22:56:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 00:25:16 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:25:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 00:25:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 00:25:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 00:25:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6c67ddc305b7f97a531083e369316343b3d19da2352e4e3274db751bba38e2`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 272.0 KB (272047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8a37c8e9266706ee6b9ca75c42931dfe1320723ad6a20f0ad4c97554998348`  
		Last Modified: Wed, 25 May 2022 00:59:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a482f319cf9a81f236c51c53bb1c689e8b1fa579667d51ca5ed246ee842f0e`  
		Last Modified: Tue, 12 Jul 2022 22:35:48 GMT  
		Size: 111.7 MB (111655243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9920ad3da4e1bfa17727a4264ec8048f45c5117be4799010b8a718e4004cd91`  
		Last Modified: Tue, 12 Jul 2022 22:34:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3afe0ff63358ebff72e63d2f0e98d572f7b7705859c43e57f9ef9cfb8447237`  
		Last Modified: Tue, 12 Jul 2022 22:57:30 GMT  
		Size: 6.8 MB (6806683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8e293f9d738d252bf475ce912e8291238915bf42ce57e839482143ab0287d`  
		Last Modified: Wed, 13 Jul 2022 00:26:43 GMT  
		Size: 1.2 MB (1229160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5f7917a376356834c38ec70309cec40192a27123e32b1516ccdf50a3de64a`  
		Last Modified: Wed, 13 Jul 2022 00:26:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4d18ee072281fc258a9eb19957ead3c8465339eb7b1f5f269afdb3bc9ad4fa09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121402125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf6e75b9e1db747dea3dc9c073f2ecaffbce977107e2c900a2163fbdb0297969`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 03:51:19 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 03:51:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 03:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:40 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 01:20:33 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:20:36 GMT
WORKDIR /go
# Thu, 14 Jul 2022 04:51:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Jul 2022 04:51:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 14 Jul 2022 04:51:15 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:51:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Jul 2022 04:51:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Jul 2022 04:51:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Jul 2022 04:51:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e4e5a89e8a0366f9710ba7cb04de284f11234b8cb3dba3e69e35a76dd1c62`  
		Last Modified: Wed, 25 May 2022 04:03:05 GMT  
		Size: 271.0 KB (270972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b879ada9b059c6167f45b720f44118516dfc73e29b727218447700619fbc5`  
		Last Modified: Wed, 25 May 2022 04:03:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e1c3c4b2486777cff8d39eaf101ab399597d87ae5c000dd7b7ad510d46797d`  
		Last Modified: Wed, 13 Jul 2022 01:47:48 GMT  
		Size: 111.4 MB (111423439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309d1e7915b7277aa2caa1a4fdae40f2ca49b928d9fec95e663f3a5711b45e6`  
		Last Modified: Wed, 13 Jul 2022 01:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfb02347c7d72c96558b8bb46a4f048d1e45182f13e10c0e83edf22747ea95`  
		Last Modified: Thu, 14 Jul 2022 04:52:44 GMT  
		Size: 6.1 MB (6067337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e3c4142f91b38c3b1e65fd6fb6ef9628dcc3556482e762152e8c9d1d3c20d`  
		Last Modified: Thu, 14 Jul 2022 04:52:42 GMT  
		Size: 1.2 MB (1228015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686a634185cb5f4c2d9dba579c1eb3beebb78e69bd25447da60ac8409e08766`  
		Last Modified: Thu, 14 Jul 2022 04:52:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:290cfd704a23c2ddcb1f182f2f17674fdcdbeaeb62282475cfaeb2dcaae9af7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e226abb8bbf011ea45e449c5070530a1ef1cc1df8f81f78ffe8324696cdf73d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:40:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:40:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:40:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:25 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 12 Jul 2022 22:24:55 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:24:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:24:58 GMT
WORKDIR /go
# Wed, 13 Jul 2022 09:10:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 09:10:54 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 09:10:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 09:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 09:11:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 09:11:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3192eca97ce26527d2bdbb26d1130abcc1c9dd7b800ce2fd14619fa422640`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 271.7 KB (271711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a050256f5b6fc0800b8ae0d96e136745091c36ce8e53ba74d8ab3eed65966a59`  
		Last Modified: Wed, 25 May 2022 00:45:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c4cc194face1e292d4841acf35c12d3d21a64fe5cfa594ab6dc52873073ab8`  
		Last Modified: Tue, 12 Jul 2022 22:33:47 GMT  
		Size: 110.3 MB (110292574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685667e0af253c6086e8398208c7561561541b211e9ddbbcf4ef6be883686ef`  
		Last Modified: Tue, 12 Jul 2022 22:33:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db124a84d37b8773dd6f7f3dd17698fb5775f4f372998d4594652b36951c51ed`  
		Last Modified: Wed, 13 Jul 2022 09:11:45 GMT  
		Size: 7.1 MB (7051424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369ee509a95002753f22f52015b6d73f187734670231017a28315b2e679616d0`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c79b21287a253cbeff92e71a14c553de9540b34d770e268a8516fa4aa873e8`  
		Last Modified: Wed, 13 Jul 2022 09:11:44 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:45efd91580c564bafa163224d57cea1742c852d9dbcacc2458d07f2766222c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122018553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe6a5f3afb3907fcc50178a016518559167b721a37de228f9c66eb515bf066f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:17:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:17:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:17:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:04:48 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 05:08:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 05:08:16 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 05:08:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 05:08:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 05:08:32 GMT
WORKDIR /go
# Wed, 13 Jul 2022 22:11:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 22:11:13 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 22:11:14 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:11:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 22:11:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 22:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 22:11:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c1f83aeafafff903bb460e7e24594fe138ebceeb1b56e898cf0158ea3daaf`  
		Last Modified: Wed, 25 May 2022 00:27:59 GMT  
		Size: 274.2 KB (274180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8365966bf1e6bd302f9e7c3d8e027aef3cfab1652ed22b8bd53311ef9517f0d3`  
		Last Modified: Wed, 25 May 2022 00:27:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a10ac130bb3da5c68d2d1ddd0bddd9c9aafed7a843450be82de6d7afbf936b`  
		Last Modified: Wed, 13 Jul 2022 05:39:52 GMT  
		Size: 110.3 MB (110295902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1b6a1686a88fdc83aa69e21aa8af36292281aded76e23d6478ea562dc6f96`  
		Last Modified: Wed, 13 Jul 2022 05:37:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f614e9e2e974dc8b16c5a51ac52e34a0134a1d53aafdb0b3f5cfa4b5d2856fc`  
		Last Modified: Wed, 13 Jul 2022 22:12:38 GMT  
		Size: 7.5 MB (7481646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94763b8678030186e0f46988e42fc162735c88413e46aaf5ed2a4956f39dd44`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea48a0db2f2ebe6c442a9a51b0febfdd54d1baf5924bc7cb12b54ae2011796d`  
		Last Modified: Wed, 13 Jul 2022 22:12:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7903fc94e9870b09a5c16e5ef6afc2ccb73eb64a00028d57a0a8b954c7d36a3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124314762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7170749c53aeec1e443a594cab8e6d8ae65cf4dbd937ab548ffaf95dfefedf94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 00:41:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 25 May 2022 00:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 May 2022 00:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:35:10 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:37:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Jul 2022 04:38:12 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:38:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:38:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:38:14 GMT
WORKDIR /go
# Wed, 13 Jul 2022 12:23:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Jul 2022 12:23:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 13 Jul 2022 12:23:06 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:23:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Jul 2022 12:23:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Jul 2022 12:23:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Jul 2022 12:23:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e497ff1a375465e6a6ba78259a6f2e9f7986cf27789ba79ddfd1cca023a160`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 272.2 KB (272155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e413365aa9b9c967651e3a27f41641db43d81f24ff58ea4de0ce2c662c5d5f`  
		Last Modified: Wed, 25 May 2022 00:50:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0da7506b596726f522d72670637523b1f1601e15dc1dd4cb1be338164021b`  
		Last Modified: Wed, 13 Jul 2022 04:56:57 GMT  
		Size: 113.2 MB (113165463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b78cd6c9206bd154e2ee3a37419413d222f10a31c24af3882cbe40c976c6016`  
		Last Modified: Wed, 13 Jul 2022 04:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15666b0ca68b6455e83f584a5eb1e817b064585023d7a42f80f62a857ae83ec9`  
		Last Modified: Wed, 13 Jul 2022 12:23:56 GMT  
		Size: 7.1 MB (7052809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa673a9dcaa66c8c1003f2b6df47b953e6e58b37233265f1949e78286795d385`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 1.2 MB (1243127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a95a05c45b1aa5d96976995433e8b8a21d81800acaf6535149cdfd51817d5ca`  
		Last Modified: Wed, 13 Jul 2022 12:23:55 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:343a268d45b94fb60575c5a477f4cf3a62b24e1c1dc6c63a25488c4871c98c69
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
$ docker pull caddy@sha256:2bd3f77e2d21db96ae5a1decdb8df220d98b96e7b812cf7d368828b16bf65ae6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99e5e593f69a4c70d75271117799e5796754e07429560f8f70a6a62a9c09b8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 07:46:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 07:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 07:46:54 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 07:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 07:46:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 07:46:57 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 07:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 07:46:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 07:46:58 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 07:46:58 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 07:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195e97acbd9f5678e292401c0fae3db777aff49e77f38d9cc3f101265b4cdf43`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 291.6 KB (291593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b702741191d81f669709a2af927df34f91029d7bdee74215cf2c65f2270cd`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6330f4d2e50b7bf2126496a3e12ab164af1ad5972222a6dd6ad58fd449b11fe`  
		Last Modified: Wed, 13 Jul 2022 07:47:23 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acec8070f9fa557cb093f66f0b2af0db792a0452918c52d5528fcb4588ad492`  
		Last Modified: Wed, 13 Jul 2022 07:47:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:71bdbcc7ee7d24783e2cf57be294f8c15b313f9c24f41ee4bf4f442c97dc8ba0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b22970098c4484f2b4a2c0d563cd0856a595d830bf660a6790517a3e6dc0c04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 00:24:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 00:24:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 00:24:47 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 00:24:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 00:24:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 00:24:54 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 00:24:54 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 00:24:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 00:24:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 00:24:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 00:24:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 80
# Wed, 13 Jul 2022 00:24:58 GMT
EXPOSE 443
# Wed, 13 Jul 2022 00:24:59 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 00:24:59 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 00:25:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c75bf2949196f38f164b182514870806879c33b90ec192cdedc33beb7164f3`  
		Last Modified: Wed, 13 Jul 2022 00:26:20 GMT  
		Size: 291.8 KB (291823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e9fed1085fb888faddfae5023a802bb85f365cfde9aacc7b2cf25064c0a7d`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d79f4f39a3e95ed2ada99510758a8816e4ddcf160793887df642ea34d47d6`  
		Last Modified: Wed, 13 Jul 2022 00:26:28 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099d09b43e9c3fdfbe6250cc5340915853372077bf3606d33ba1b9c5bad5c38`  
		Last Modified: Wed, 13 Jul 2022 00:26:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1db5af09e7e93ccc64f39d2aefa6438f3346a62fff17d5f006eef3bf5541424
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3d980491df522f57fa63138e24e8c6be022acb10104bab97857a4eab9d04f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 14 Jul 2022 04:50:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 14 Jul 2022 04:50:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 14 Jul 2022 04:50:42 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 14 Jul 2022 04:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Jul 2022 04:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Jul 2022 04:50:50 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 14 Jul 2022 04:50:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jul 2022 04:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jul 2022 04:50:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 80
# Thu, 14 Jul 2022 04:50:54 GMT
EXPOSE 443
# Thu, 14 Jul 2022 04:50:55 GMT
EXPOSE 2019
# Thu, 14 Jul 2022 04:50:55 GMT
WORKDIR /srv
# Thu, 14 Jul 2022 04:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d2eab8b066328ae05bd108fd3d593cfea00c0c5b4a920788ae29400dfa4fc`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 290.8 KB (290762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e007f0123b4d81f10149eb27d05581180511d1b2884e9f286496e20935f56453`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35e23b17501f974f98785b56b4286fedfcb3e968b0564292daec9ecd9451e`  
		Last Modified: Thu, 14 Jul 2022 04:52:27 GMT  
		Size: 13.3 MB (13347758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafbc25b5d1376069d3e359ea4fb05678d63a4a0d20fdce60afc005cfbf344e9`  
		Last Modified: Thu, 14 Jul 2022 04:52:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e277f1e570bb65d07ca7ddaf11bd50b8f64643b579e2a1500165d0d10e873b22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15720992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ab296123268f045db4f04fdd9542ea39cf0869b8a5790b52e8359cf4301f2f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 09:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 09:10:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 09:10:27 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 09:10:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 09:10:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 09:10:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 09:10:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 09:10:33 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 09:10:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 09:10:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 09:10:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 09:10:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 09:10:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 09:10:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 09:10:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 09:10:41 GMT
EXPOSE 80
# Wed, 13 Jul 2022 09:10:42 GMT
EXPOSE 443
# Wed, 13 Jul 2022 09:10:43 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 09:10:44 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 09:10:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e2632fbf469bd4459a122146d4f5c544524b9917ebbb1c82ca604c846e6d03`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 291.5 KB (291462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136b5c9b9f23df66b6049078ee2f4df8231ed7eb7f543cc31055c0c338074a3`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d759768dee9c2f0e5c5353760cb5d7fdb641c3bbc7160a9ef0e1428a504a820b`  
		Last Modified: Wed, 13 Jul 2022 09:11:30 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f38216dc74dd3541e3282c41fd26512f9161bbc74eb0fef8374f88c07c33f`  
		Last Modified: Wed, 13 Jul 2022 09:11:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:8bf33283df3ab62c0987b87b518be60e587e8e8f492f9001c9f513126218c3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b6dd61b467dc78c47f12742f5af2367935a9ffb8f6dcc8ce8382764c2d1ab8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 22:09:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 22:09:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 22:09:55 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 22:10:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 22:10:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 22:10:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 22:10:18 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 22:10:21 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 22:10:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 22:10:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 22:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 22:10:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 22:10:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 22:10:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 22:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 22:10:40 GMT
EXPOSE 80
# Wed, 13 Jul 2022 22:10:43 GMT
EXPOSE 443
# Wed, 13 Jul 2022 22:10:44 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 22:10:48 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 22:10:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49126cc0b1f1c1e51c05b6d7443ed73b5fd2577d177ced4eb36ba827a6b9e68c`  
		Last Modified: Wed, 13 Jul 2022 22:12:19 GMT  
		Size: 293.9 KB (293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f5f92095cf2a8c6afe25b29ea21344778855b89f160fed628effd01704c1c2`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12fbf7d78c1725ab5956092ae9577b979994dc526cbd9f8368c69ce317b692`  
		Last Modified: Wed, 13 Jul 2022 22:12:21 GMT  
		Size: 12.3 MB (12309531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905929de5f23fe3fc6a3b51fc5e5ae5d69bb42d68a20069887fbae365e82fba`  
		Last Modified: Wed, 13 Jul 2022 22:12:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:f3f1634a0c819eb255025ed4f6ed0cf373cf040b4433b99e741b9f356c24f035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db99049e35d90916167a13c53576818e74e4b0f30b57123b9f866b7712c8305b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 13 Jul 2022 12:22:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 13 Jul 2022 12:22:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 13 Jul 2022 12:22:45 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 13 Jul 2022 12:22:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 13 Jul 2022 12:22:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 13 Jul 2022 12:22:50 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 13 Jul 2022 12:22:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jul 2022 12:22:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jul 2022 12:22:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jul 2022 12:22:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jul 2022 12:22:53 GMT
EXPOSE 80
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 443
# Wed, 13 Jul 2022 12:22:54 GMT
EXPOSE 2019
# Wed, 13 Jul 2022 12:22:54 GMT
WORKDIR /srv
# Wed, 13 Jul 2022 12:22:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a278a0c4f266219ec8afd82734a3a15f7ad274e786c5e813adde536d23e7a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 291.9 KB (291943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bfcbf66ce9f538fed4132cec8e97597e9ace9340502c5ed98c06909e9369c9`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26380b79ed6fa2324d957b5d5f3c38ae3aaccb280e477850bdae2952a1e1c308`  
		Last Modified: Wed, 13 Jul 2022 12:23:44 GMT  
		Size: 13.5 MB (13460701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319ee79626cacd3ef26113bfb7c3a9086642a88ba734de13a93138ce13b839a`  
		Last Modified: Wed, 13 Jul 2022 12:23:42 GMT  
		Size: 155.0 B  
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
