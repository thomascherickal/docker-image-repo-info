<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.1.1`](#caddy211)
-	[`caddy:2.1.1-alpine`](#caddy211-alpine)
-	[`caddy:2.1.1-builder`](#caddy211-builder)
-	[`caddy:2.1.1-builder-alpine`](#caddy211-builder-alpine)
-	[`caddy:2.1.1-builder-windowsservercore-1809`](#caddy211-builder-windowsservercore-1809)
-	[`caddy:2.1.1-builder-windowsservercore-ltsc2016`](#caddy211-builder-windowsservercore-ltsc2016)
-	[`caddy:2.1.1-windowsservercore`](#caddy211-windowsservercore)
-	[`caddy:2.1.1-windowsservercore-1809`](#caddy211-windowsservercore-1809)
-	[`caddy:2.1.1-windowsservercore-ltsc2016`](#caddy211-windowsservercore-ltsc2016)
-	[`caddy:2.2.1`](#caddy221)
-	[`caddy:2.2.1-alpine`](#caddy221-alpine)
-	[`caddy:2.2.1-builder`](#caddy221-builder)
-	[`caddy:2.2.1-builder-alpine`](#caddy221-builder-alpine)
-	[`caddy:2.2.1-builder-windowsservercore-1809`](#caddy221-builder-windowsservercore-1809)
-	[`caddy:2.2.1-builder-windowsservercore-ltsc2016`](#caddy221-builder-windowsservercore-ltsc2016)
-	[`caddy:2.2.1-windowsservercore`](#caddy221-windowsservercore)
-	[`caddy:2.2.1-windowsservercore-1809`](#caddy221-windowsservercore-1809)
-	[`caddy:2.2.1-windowsservercore-ltsc2016`](#caddy221-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:3bdc57eb2bf54c1df10c43fc566f1cc5269f6ae8a5b9a86e3b9fa98a614a66d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:5c14834055e3ec0800789a46db92258f78556ef9971457022234e3487c2ae207
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4daabe9339412068d7bcc4c9b0ac275c67c82d8c819e4b37a387b50fa8e9a61b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:28:21 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:28 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4428f13c7edb68201eb53fc2a833e3e1831b1bfc66d8ca591d7d7981e8dcdb57`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b931870cc5c313c5b12bd911762577180c41684025e803ac19870628f24474`  
		Last Modified: Fri, 11 Dec 2020 02:29:11 GMT  
		Size: 11.5 MB (11532507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010bdd923cf20d340b6e9f06cac8c3f1e1984172c4f4d095cd9b443b03ad818`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ee965d543057e5cb4af597d364066251a9852583059cd38488243306b724a778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7753d72769487802d1fee3d3f07ee3ce735418d63d93259ad8125a3ae2de1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:10:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:10:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:10:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:10:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:10:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:10:21 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:10:21 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:10:22 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:10:23 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:10:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:10:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:10:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:10:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:10:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:10:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:10:31 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:10:32 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:10:33 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:10:35 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:10:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7ab50db8ca6e467811f1281518708c79ffb3eba857ede634fe075aa109cf4`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c5497e98ba2efc52fb51339d08617c1ffc210163f8774632f307c81683deb`  
		Last Modified: Fri, 11 Dec 2020 03:11:27 GMT  
		Size: 10.9 MB (10876275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140a3a819ce00971b2089202730b7c285ca9a6ab1f5832820b20a043fd51fcc9`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2d82fb7e660d56846fa3c33deb953bfc6c464bfb8fba608c237b4a5e0eee33c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e57be32d04a04308b9f9c3fcbac701e798783ecbe10f243a411262f5a05cb0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:07:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:07:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:07:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:07:14 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:07:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:07:16 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:07:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:07:18 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:07:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:07:24 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:07:25 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:07:26 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:07:27 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:07:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2348443ed0fb4b09e2d5b6d636d90e4bbf2024e934143fadfcc35bbc65a709a1`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8462380e6876aca9643bcf369ffc7b958a08c3fd3fc56a861ca651a1fcaf9c`  
		Last Modified: Fri, 11 Dec 2020 03:08:19 GMT  
		Size: 10.9 MB (10854381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7839ddc84cd5ea73da141c2726d80c7493a37772c128eb7f60b1621784acf0`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8a8a108facaeb348bc873b80764a0e142fa06279dce55fc16f6d68017de99f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b781915644b6cb14f7dbcb44242df9845f6f989c96c3b75da745a4c11d116ca0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:33:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:33:42 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:33:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:33:52 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:33:53 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:34:00 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:34:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:34:03 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:34:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:34:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:34:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:34:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:34:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:34:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:34:19 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:34:21 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:34:23 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:34:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a6157741b4baecc6781d3a2227bd753df1a152366cfba7d5f83731611b38f3`  
		Last Modified: Fri, 11 Dec 2020 03:35:17 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f6d968230fb7b05d7bb6b35f8eab026c6e68c93458a9c40095b9bccb7eb23d`  
		Last Modified: Fri, 11 Dec 2020 03:35:20 GMT  
		Size: 10.5 MB (10527460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665b752f90ad5d8f5f8c6840c5cc58eb1b542c21773b827303c156732f73321`  
		Last Modified: Fri, 11 Dec 2020 03:35:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:b5c5d0c317892db3c940899c940405ad1283f0857b3cb1c454abce45a325b8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf8c3b1e29b5c01bce118fbc104af2924a4b50324db40dedeb78ba2d9df4c33`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 06:44:22 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 06:44:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:44:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:44:48 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:44:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:44:54 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:44:57 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:45:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 06:45:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:45:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:45:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:45:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:45:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:45:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:45:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:45:35 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:45:39 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:45:45 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:45:49 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:45:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f10029b2ed0c8a52065e9b56b5b27d4f7a83fcba0392c7021532236b70a0f`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd4c79b504a226097858b4a8bc37dbed1031f3a3205cf552a5ebceb132f791`  
		Last Modified: Fri, 11 Dec 2020 06:46:51 GMT  
		Size: 10.2 MB (10180214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2cc34795b6c9d9081692bd53a1f7b77ae6a7c9e9e661f863cc493d6973a26`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:90b5dcd8d713f82a46c2039baee451f911f8d25f27431e6b44655f8b2803c557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f49a1c397b4a9cdc0f9a6cd1eb6aea12154952a3d4ead09ddd6c9595bb4361`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:43:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:43:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:50 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752f95e37b35ec8cf81bd3caab7ba2ea836620747fa2d720c5b64709254ddae`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f574024c894c439da18a68fa9e20ef03be94dd77a2b1934242463f93d518b0`  
		Last Modified: Fri, 11 Dec 2020 02:44:34 GMT  
		Size: 11.2 MB (11202556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26947b55683beda16dec6f01fc3ef037d91c61349dae0527952bafce3c03d5c0`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:7a3324e3c17ab6ca575fd9957ed7d0b381a49bf9a99e23e82f3605e49d6a4f8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.1.1` - linux; amd64

```console
$ docker pull caddy@sha256:c15ad866555b509b7e6133835f65b837e0e45c743c66327919b82efd7d39f39a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f92074db62da370b0a009b24f119bc15c52c0147443e6540aefd9af48c46469`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 02:28:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 02:28:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:08 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:09 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:09 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:09 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 02:28:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:11 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:11 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:11 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:11 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5390499a3f77123738116182f93488c8c2a2c2c96737041df127367f0ed8619d`  
		Last Modified: Fri, 11 Dec 2020 02:28:59 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a9fcf243885eece7438e6da948cbeb42422ec0fe93af5e953f8ea3320d0554`  
		Last Modified: Fri, 11 Dec 2020 02:29:03 GMT  
		Size: 13.1 MB (13057344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cfbf56ec3778ab1fa6053909ad354e23f0e152b688f5210bb0c5666fb1f0c3`  
		Last Modified: Fri, 11 Dec 2020 02:28:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0643a46228552f6f8371abb3bced8a2d037067f36e690e1fd6279375ab850d01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15323010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84b6a1dd8e839352d9684e0815ae89594252f9a40330cd80812f2de1f8fdd46`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:09:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 03:09:35 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 03:09:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:09:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:09:43 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:09:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:09:45 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:09:45 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:09:46 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 03:09:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:09:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:09:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:09:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:09:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:09:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:09:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:09:53 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:09:53 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:09:54 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:09:55 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:09:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc374dd2fd1d2486f9f660080d64e7565d74e310d219c93d33b19619fe7f30b1`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5d2c8d0ac42e5f41eb7f3dda6f59cc61f09a097dd5333305d2d20c2ac51268`  
		Last Modified: Fri, 11 Dec 2020 03:11:17 GMT  
		Size: 12.4 MB (12414921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764d3fd050ed3fbe5a55400dd03a3016953eaa56977be967e70829cec93388a1`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02d4fcd8ac4463653a4752f7f74e4d0f3c74ade1d1bf0bf1abdc0f4596927b11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15106917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f62dfafb3c9a9e5fc3d3475555fae59332a59615514c37cfe2a1d91bcdad66e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:06:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 03:06:29 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 03:06:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:06:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:06:38 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:06:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:06:40 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:06:40 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:06:41 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 03:06:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:06:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:06:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:06:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:06:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:06:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:06:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:06:48 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:06:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:06:49 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:06:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:06:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22200112a218516c5d9d0e69d1f2e1ecd19e9d1cc6129431a2cd744858ad0a33`  
		Last Modified: Fri, 11 Dec 2020 03:08:01 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1fa647166950f21caa9a62eae0491f26f21892129d7e4d6872cf1cc26cef93`  
		Last Modified: Fri, 11 Dec 2020 03:08:05 GMT  
		Size: 12.4 MB (12396042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ea9281180fac696ccdf854264daeef5f54b4e980b7dbd3ff5c36ad65f7bbea`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:63d22097b436e2dd3c0929493ee7c4eadaa2b6b27c1a278caa32841849afc794
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15026050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c53097798daadcccdb683b4ce0a6dd67dd325c01b6ee9a0db1e51a86117eeb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:32:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 03:32:24 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 03:32:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:32:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:32:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:32:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:32:48 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:32:49 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:32:50 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 03:32:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:32:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:32:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:32:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:33:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:33:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:33:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:33:08 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:33:09 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:33:10 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:33:11 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:33:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425bbd647135b24a8e3c6cb25cb7c3ef22c4513013aefdc57c41988e20f421c`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1435586584b1cefb2a0cadc47752d61799ec51e54cb01485f004e8dd9b7633`  
		Last Modified: Fri, 11 Dec 2020 03:35:07 GMT  
		Size: 12.0 MB (12013108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273417eb816e43856d6b60380d90601b2235f0a15efa6bf6228008379b160f0`  
		Last Modified: Fri, 11 Dec 2020 03:35:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:4ea85095f24b5ecd2e9494128ca73fa7d06c4aaa28ff9b6adaa28171c4a25df1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14897192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fb7c7a447c300146a1040945bbb693d7e466d338c8107ac74eebce3340ffe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:42:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 06:42:17 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 06:42:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:42:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:42:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:42:51 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:42:55 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:42:59 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:43:02 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 06:43:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:43:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:43:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:43:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:43:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:43:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:43:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:43:37 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:43:41 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:43:48 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:43:56 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:44:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47c0280031fbe4262af27a47c4efc973e07d463cd5e2971f853cfd9811cac92`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fb89cea813d254396a0133c87398f5d6f1623970ee81f8a6cb272ae316d53`  
		Last Modified: Fri, 11 Dec 2020 06:46:38 GMT  
		Size: 11.8 MB (11785447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ede4bf59064aa7de718cd57d1bafb6d247adcbe8ff2f33c9a9b66553f534e3c`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; s390x

```console
$ docker pull caddy@sha256:3061e8cf3b1d5602dd74cd289d1e5d5cc337b3a351650ab55729198a6e86993e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2a1ae7d615bad4d37c8062c88bfed52c362c6bcd10d61cccd9349f54804551`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 02:43:04 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 02:43:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:12 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:12 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:12 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:13 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 02:43:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:17 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:17 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:18 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:19 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb92280db540f0ef28cb2a919c84d8bb234581ea3dc170be764578581e854dd`  
		Last Modified: Fri, 11 Dec 2020 02:44:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04542cfd874bde71e1eac0011031135c9f9a7764b9680db69831eaf7b0c9b7a9`  
		Last Modified: Fri, 11 Dec 2020 02:44:26 GMT  
		Size: 12.8 MB (12836810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eae3acd51142f8c949369808f4302d04048381914dc707b31df353246b1863d`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:9a3bcc6076982ff8b0833a250a3bdec2f0fc180d3869a50df2c5111c35900756
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2418118741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eabf81561f405d4bdf2b4704d6ca869edc7ddea014dd1abe0f360edb2f249ed6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:42:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:42:47 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:43:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:43:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:43:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:43:23 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:43:24 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:43:24 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Dec 2020 22:43:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:43:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:43:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:43:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:43:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:43:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:43:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:43:30 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:43:31 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:43:31 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:43:47 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:43:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8310e6a3befeed4407572cd52b3887e0fda9b586ca388d76f9e9e14f0174d6`  
		Last Modified: Wed, 09 Dec 2020 22:58:23 GMT  
		Size: 9.2 MB (9243060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e21e51fee4a54f410d2f26105f8ee67030de4d0c2f7e977ac39a5635f093c5`  
		Last Modified: Wed, 09 Dec 2020 22:58:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24348cbc7752073f17d52670e5f5678337f4f518ae178cc70a98daaab1b3b4`  
		Last Modified: Wed, 09 Dec 2020 22:58:24 GMT  
		Size: 17.7 MB (17701596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6652d297bd09a384ff9270741baf15f8273217c718aae1a2b722fde0354fab17`  
		Last Modified: Wed, 09 Dec 2020 22:58:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f68b024395847bee888c4527f15e46931af7c4b33eba653fe6b3e5f91d90bf`  
		Last Modified: Wed, 09 Dec 2020 22:58:18 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5c45ff80ddf22adcfc93ef960cbc1fb6389e7b836abb8a29ec0fed22ac25`  
		Last Modified: Wed, 09 Dec 2020 22:58:17 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92e3d73352785cfd5be7f16932b53670b41691d227980cd835bf418f14d8a82`  
		Last Modified: Wed, 09 Dec 2020 22:58:17 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6f5bbdfb82b660d77e1075f9af7110b7bfe9f6708c60f15f8aa2df164b45ee`  
		Last Modified: Wed, 09 Dec 2020 22:58:16 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974f29c0c664d8a7edccac5aea85146f0c28f08450b89315bac02e12bcb803c`  
		Last Modified: Wed, 09 Dec 2020 22:58:16 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7a2fbf68d6d2c48d7221407dbf9de908850675adef8e05da13dcfdd889f2b1`  
		Last Modified: Wed, 09 Dec 2020 22:58:15 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab33f16822bafab6e4e5d8cb0239224fa9ded2b36ab1f043c58ee1090ffffe5b`  
		Last Modified: Wed, 09 Dec 2020 22:58:13 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b973cee99b817a2b430e8b288d5bbf5345a86c7a8bc7478db3bb7a06fc8a08f`  
		Last Modified: Wed, 09 Dec 2020 22:58:14 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f9be9ebe03c3c6264d1187eb40cf64cb2e3a0797b9c7d7020fe89e7446b3`  
		Last Modified: Wed, 09 Dec 2020 22:58:14 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f928962368a43603f41dd1b4d7cc013507a02b94a0c04b895f9b36a95b2d69`  
		Last Modified: Wed, 09 Dec 2020 22:58:13 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266811a4d21e656edad5a4620f4665d9af80a27efcf1939e3e421f9dc5be643`  
		Last Modified: Wed, 09 Dec 2020 22:58:12 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06371064917888a8d76cf047c3d638ab2c47c1d1455af625e5328dfe7ccd9106`  
		Last Modified: Wed, 09 Dec 2020 22:58:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeb1400c5654b601c27186e5d01a98b7edac4e1eab9e685a72a5b76e051b649`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643137612c3791ba413e0c82a6ab3a7bfc9e0f63d12606aa5100a601e5537867`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ebbab633b643578785da16143e2bea1a1e3a0a084a69bc3926b7874f6f0b4`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 279.1 KB (279142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec87bc08f9747fe4d23aa34857acb63e17bfb53f1c218b84c375528171675bc`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:bef89cd4397dfc72efac26c3af66c367167de1f7beb5fa15b9eb16103d69edfd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802183304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27357e1c65458f12556946c0756fa611e58dd1e58fce5e1d3c744cfc6ad3d26d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:45:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:45:21 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:46:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:46:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:46:47 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:46:48 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:46:49 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:46:50 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Dec 2020 22:46:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:46:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:46:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:46:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:46:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:46:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:46:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:46:56 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:46:57 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:46:57 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:47:41 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:47:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb3365d5b5f52406d1460ea71ec7dc45a0be84fb11ee92a095c01446982ac`  
		Last Modified: Wed, 09 Dec 2020 22:58:47 GMT  
		Size: 10.1 MB (10058753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7e40284fe73310de6916db9588492c76d9faf162ba20cc75e06f28cdf5b5d3`  
		Last Modified: Wed, 09 Dec 2020 22:58:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d808c13287b5d9fe34c6cc197e3a5f1c625583988ab9261ad38969f3b3bb727`  
		Last Modified: Wed, 09 Dec 2020 22:58:49 GMT  
		Size: 23.0 MB (23021357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0327ccf8c96f9c862dcbb6a7b88a7834597610a976c6a1a0e5b6e60705337019`  
		Last Modified: Wed, 09 Dec 2020 22:58:42 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45aa920e303bd017aa55620871520648cd55969ae89963b8180cf8462a06d9f`  
		Last Modified: Wed, 09 Dec 2020 22:58:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06dc416d5acc13c105dfb12dc601bf956d10efef6ef96d5639fdba94d236762`  
		Last Modified: Wed, 09 Dec 2020 22:58:41 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad9f0882cad71b6b14c48e7ffa0ca9b90bb89d577097f1cb2f7892cb1fcb780`  
		Last Modified: Wed, 09 Dec 2020 22:58:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e4736002f89abfa7f6da14661a1f6a4d2ae079c3f31102bffe18cdd8beeb6d`  
		Last Modified: Wed, 09 Dec 2020 22:58:39 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86169177264c9317107ac0a5ca73674c2de958677546206af268ee1f54dd084`  
		Last Modified: Wed, 09 Dec 2020 22:58:39 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5448bd5ec4e8f017b5a6ad026679927adffa04f4cad61f078dad05f5698afd`  
		Last Modified: Wed, 09 Dec 2020 22:58:38 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fc40c7d9ddfd83bff64476793cb83f8f16c29f719ef4ac1ab472ccfd21527a`  
		Last Modified: Wed, 09 Dec 2020 22:58:37 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69dd9ca0f7b2f5dcd5a208296f33e5b2e918b471971464afecaea0528dca320`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1467e2c551c61df53878d778d60d4206f2b0985166be921d43025fe9eea9a617`  
		Last Modified: Wed, 09 Dec 2020 22:58:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ffdf83969e06a380e2e5ad6d6e247cecf5ab242f9388917e95c3cb442a087`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb4589051190d97302d6ec12f716820272f7c07dac4e4a3cf2685ec1d4404c`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb4bdcb4f4f977edee7bd1de9042084c67eb27db3c8a820f6e463da7c6198e9`  
		Last Modified: Wed, 09 Dec 2020 22:58:33 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bec2c9e631017e4bd85ef16b73b059ae9dcd2d65e96093e91332872b4a484d`  
		Last Modified: Wed, 09 Dec 2020 22:58:33 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdf38a5e62965ddd16e787d39db0033eec3827e459ed8c8b8edd00b2742ba3d`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf1879d55948e8a6692625974f1ce349eb596a2ee5fae7442503b720ffe6768`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 238.7 KB (238665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79a4b2f0acee85ce6edc7959ba4733df596c028ad2e07d6626581d716531869`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-alpine`

```console
$ docker pull caddy@sha256:379a0fccfa549ebcde668bdc5bf4d863847680159161de48025344c813143b68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:c15ad866555b509b7e6133835f65b837e0e45c743c66327919b82efd7d39f39a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f92074db62da370b0a009b24f119bc15c52c0147443e6540aefd9af48c46469`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 02:28:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 02:28:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:08 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:09 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:09 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:09 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 02:28:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:11 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:11 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:11 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:11 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5390499a3f77123738116182f93488c8c2a2c2c96737041df127367f0ed8619d`  
		Last Modified: Fri, 11 Dec 2020 02:28:59 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a9fcf243885eece7438e6da948cbeb42422ec0fe93af5e953f8ea3320d0554`  
		Last Modified: Fri, 11 Dec 2020 02:29:03 GMT  
		Size: 13.1 MB (13057344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cfbf56ec3778ab1fa6053909ad354e23f0e152b688f5210bb0c5666fb1f0c3`  
		Last Modified: Fri, 11 Dec 2020 02:28:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0643a46228552f6f8371abb3bced8a2d037067f36e690e1fd6279375ab850d01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15323010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84b6a1dd8e839352d9684e0815ae89594252f9a40330cd80812f2de1f8fdd46`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:09:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 03:09:35 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 03:09:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:09:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:09:43 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:09:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:09:45 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:09:45 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:09:46 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 03:09:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:09:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:09:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:09:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:09:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:09:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:09:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:09:53 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:09:53 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:09:54 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:09:55 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:09:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc374dd2fd1d2486f9f660080d64e7565d74e310d219c93d33b19619fe7f30b1`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5d2c8d0ac42e5f41eb7f3dda6f59cc61f09a097dd5333305d2d20c2ac51268`  
		Last Modified: Fri, 11 Dec 2020 03:11:17 GMT  
		Size: 12.4 MB (12414921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764d3fd050ed3fbe5a55400dd03a3016953eaa56977be967e70829cec93388a1`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02d4fcd8ac4463653a4752f7f74e4d0f3c74ade1d1bf0bf1abdc0f4596927b11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15106917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f62dfafb3c9a9e5fc3d3475555fae59332a59615514c37cfe2a1d91bcdad66e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:06:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 03:06:29 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 03:06:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:06:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:06:38 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:06:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:06:40 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:06:40 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:06:41 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 03:06:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:06:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:06:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:06:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:06:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:06:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:06:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:06:48 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:06:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:06:49 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:06:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:06:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22200112a218516c5d9d0e69d1f2e1ecd19e9d1cc6129431a2cd744858ad0a33`  
		Last Modified: Fri, 11 Dec 2020 03:08:01 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1fa647166950f21caa9a62eae0491f26f21892129d7e4d6872cf1cc26cef93`  
		Last Modified: Fri, 11 Dec 2020 03:08:05 GMT  
		Size: 12.4 MB (12396042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ea9281180fac696ccdf854264daeef5f54b4e980b7dbd3ff5c36ad65f7bbea`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:63d22097b436e2dd3c0929493ee7c4eadaa2b6b27c1a278caa32841849afc794
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15026050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c53097798daadcccdb683b4ce0a6dd67dd325c01b6ee9a0db1e51a86117eeb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:32:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 03:32:24 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 03:32:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:32:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:32:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:32:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:32:48 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:32:49 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:32:50 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 03:32:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:32:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:32:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:32:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:33:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:33:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:33:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:33:08 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:33:09 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:33:10 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:33:11 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:33:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425bbd647135b24a8e3c6cb25cb7c3ef22c4513013aefdc57c41988e20f421c`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1435586584b1cefb2a0cadc47752d61799ec51e54cb01485f004e8dd9b7633`  
		Last Modified: Fri, 11 Dec 2020 03:35:07 GMT  
		Size: 12.0 MB (12013108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273417eb816e43856d6b60380d90601b2235f0a15efa6bf6228008379b160f0`  
		Last Modified: Fri, 11 Dec 2020 03:35:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:4ea85095f24b5ecd2e9494128ca73fa7d06c4aaa28ff9b6adaa28171c4a25df1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14897192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fb7c7a447c300146a1040945bbb693d7e466d338c8107ac74eebce3340ffe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:42:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 06:42:17 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 06:42:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:42:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:42:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:42:51 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:42:55 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:42:59 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:43:02 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 06:43:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:43:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:43:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:43:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:43:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:43:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:43:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:43:37 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:43:41 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:43:48 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:43:56 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:44:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47c0280031fbe4262af27a47c4efc973e07d463cd5e2971f853cfd9811cac92`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fb89cea813d254396a0133c87398f5d6f1623970ee81f8a6cb272ae316d53`  
		Last Modified: Fri, 11 Dec 2020 06:46:38 GMT  
		Size: 11.8 MB (11785447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ede4bf59064aa7de718cd57d1bafb6d247adcbe8ff2f33c9a9b66553f534e3c`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3061e8cf3b1d5602dd74cd289d1e5d5cc337b3a351650ab55729198a6e86993e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2a1ae7d615bad4d37c8062c88bfed52c362c6bcd10d61cccd9349f54804551`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 11 Dec 2020 02:43:04 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 02:43:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:12 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:12 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:12 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:13 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 11 Dec 2020 02:43:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:17 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:17 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:18 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:19 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb92280db540f0ef28cb2a919c84d8bb234581ea3dc170be764578581e854dd`  
		Last Modified: Fri, 11 Dec 2020 02:44:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04542cfd874bde71e1eac0011031135c9f9a7764b9680db69831eaf7b0c9b7a9`  
		Last Modified: Fri, 11 Dec 2020 02:44:26 GMT  
		Size: 12.8 MB (12836810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eae3acd51142f8c949369808f4302d04048381914dc707b31df353246b1863d`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder`

```console
$ docker pull caddy@sha256:60944d00c87ca4d9b0b62338772a2b18793fd62bb26e0a6547437ae255759910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.1.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:37c634e75d14fc942393b95a9ca1803bc2e6eb39276cdbcb41f04653eb1aca3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120346515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3c25baf9316333b4308baa85ff5c4f5bdcdd0f2b43f480277a2427e10d43c6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:25:03 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:27:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:27:20 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:27:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:27:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:27:22 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:48:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:48:55 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:48:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:48:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:48:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff250548074e76394d085b3a57acccc88c05cbde1dbb4b27f7a7d3f752d1df0`  
		Last Modified: Fri, 04 Dec 2020 00:32:49 GMT  
		Size: 107.6 MB (107550990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c86fa391e3d32b3d1db825e61ae70f87831992751d5971c62c587526b7909cb`  
		Last Modified: Fri, 04 Dec 2020 00:32:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f309d33d760b2353f1b3cb1949ec8696c5076f42b245ae14aa1a1976fb8ab`  
		Last Modified: Fri, 04 Dec 2020 00:49:38 GMT  
		Size: 8.3 MB (8309953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a78bef7d8825ad6c9b092e9a9151f84af560335cd3492c3cd800bcf829eabda`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 1.4 MB (1407215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ee2ac4bf7c1c60fccb631b07fc1371698f356b1bf848be393ead9c77914e1`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f4427023da794f7d46eef3fe23cc301a5ef9c4874e4384bbb93384d020f6f0cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115653449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6342dd6fa9a9e648434ee73c7e823cf8a90ec3c85e04666c0971fea02c6c9cf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:54 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 11 Dec 2020 05:07:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:07:42 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:07:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:07:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:07:52 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:14:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:14:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:14:33 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 08:14:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:14:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:14:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:14:40 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d14bc917e8b0e9b1e8da9e1addfea1476f1fdb73c59cfba028859bd35b6522`  
		Last Modified: Fri, 11 Dec 2020 05:09:57 GMT  
		Size: 103.5 MB (103513561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e7a785a4bea2bdefcae5d67c33482821f9fbfbad17744f3845c7fedcbf8a84`  
		Last Modified: Fri, 11 Dec 2020 05:09:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c253ffba74eeb65d966efb71aafd82bf788b9c9b9c034a1ef0ba8fd69fb89`  
		Last Modified: Fri, 11 Dec 2020 08:15:54 GMT  
		Size: 7.9 MB (7928847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5ec84babb1bb15bf1bfe449a456d7fb33928afaffe622debf4b02d9c8cb0ed`  
		Last Modified: Fri, 11 Dec 2020 08:15:53 GMT  
		Size: 1.3 MB (1327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e533154e63147025a965a7c3810aeb74085482a1424142ce76497d163a58cae`  
		Last Modified: Fri, 11 Dec 2020 08:15:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e03abef2fec55f201484597a22643a5f555b17f5bebdc057334bd7a301f424b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114812725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c2dfdfc3751b3030414e6c70bc516989641ccce757579869a633b3b31862af8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:07:09 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:09:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:09:40 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:09:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:09:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:09:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:05 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:33:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc832c4959c984d61cbf9ca04945922a7ac84d32c9a7dbfc4000f56b593f8fe`  
		Last Modified: Fri, 04 Dec 2020 00:16:33 GMT  
		Size: 103.7 MB (103655540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75782af3feb5c44682b68de6dbe1678c0028b8316b235c6bb325c9b96d47466f`  
		Last Modified: Fri, 04 Dec 2020 00:15:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3103923df4c137961411ee9beb2163bb0fceb96024cab996b338fff9dec323cb`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 7.1 MB (7144867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267c9a980b43f5e19848c54b902901643b512e49bca7eeb2694d6395d58d9e5`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95b1cb145016023a360ff49d799308bb9a33fdaa990f076ead6e8454424856e`  
		Last Modified: Fri, 04 Dec 2020 00:33:58 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c342415c2eacab2e75ff361dc7a30271d8693f36dfa5812bc9a73b45fb7650e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115766627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26fb7973448a7a127743363016ea1407c9372ff89327d196152ccb285a64d74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:02:52 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 01:04:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:04:52 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:04:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:04:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:04:56 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:07 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:08 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:28:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:13 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f038c27fba9771a10e2d17f066f31884e1d64e9d50f996d4e1f98c7d9eca6df5`  
		Last Modified: Fri, 04 Dec 2020 01:11:44 GMT  
		Size: 103.0 MB (102968080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb141fcf8afeddffe403b798e502235e8746a2bbcecb5325ae2067d6e64aedc`  
		Last Modified: Fri, 04 Dec 2020 01:11:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237402524d7a7d687e3e2866ec83f21ad5a498ed7f26f1a8236cda6b5f560929`  
		Last Modified: Fri, 04 Dec 2020 01:28:54 GMT  
		Size: 8.5 MB (8499866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c71374c7630456a387209dca122b16a8038192403356b827b0dfa2ab77eff`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 1.3 MB (1310182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6da552cad766345c3058306ad61d20a6f02651f46d71ce40583fc9f18762f7`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:a3966dfa7df24217bd14943995fc0e4d6d8084992a5c389ccbca4f4118804b22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115150516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef65b689756199e63647a98cebfe48993694a73b122f91d3be33a2d69ce7c56`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:59:55 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 02:02:08 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 02:02:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 02:02:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 02:02:24 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:12:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:12:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:12:34 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 03:12:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:12:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:12:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f63d5e2daabbfe6e2070563b812f7d8cedf414d153c493cd60bfc611e364dc9`  
		Last Modified: Fri, 04 Dec 2020 02:08:29 GMT  
		Size: 101.9 MB (101855605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07277d6b2e6785d1fc5318d4c63b413a76cb86a9d7beeb0d20bdd835d34eea19`  
		Last Modified: Fri, 04 Dec 2020 02:08:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6e1068327176aa38aa1e6a20aa01eeeb3b9427cbc0f41fbe367cc06474325b`  
		Last Modified: Fri, 04 Dec 2020 03:14:31 GMT  
		Size: 8.9 MB (8919981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86508b35ca9f1a8e0db3f8fc347a62e1e17b591a7785c85705169631d0df17d1`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50938474f3e06598b1f0264f5bc734dde207d35f09f032ddae0bcf66fe7252e2`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:eb0a6338a700322a20d0aa43f2806d21e393e6ea8223c279d2478aac22c2def6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119651264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2693c682f63cd6fcfd6ed02092b945cea78feada8d46df763f09b96776c21818`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:30 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 11 Dec 2020 03:34:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:34:24 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:34:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:34:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:36 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:36 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 16:39:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:40 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cad920206526b07e54157f3f3e750c020714ef2fa81afaf15795a370a17c16d`  
		Last Modified: Fri, 11 Dec 2020 03:35:53 GMT  
		Size: 107.1 MB (107062213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4289f50a1bbc5253453a64e5de3e8ea337aaac81e21fcef64eeeaea68d0e507`  
		Last Modified: Fri, 11 Dec 2020 03:35:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7067c7cd350e8ef505f157b1add8a9a301c34ef4504b86eeba9d327253e4c55`  
		Last Modified: Fri, 11 Dec 2020 16:40:32 GMT  
		Size: 8.4 MB (8352271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23965c15ee31da004d6acd1aeed41b837d70bb87a1240266dd2ccc6b1722f7ee`  
		Last Modified: Fri, 11 Dec 2020 16:40:33 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dccb0aaab794fa2f8fd0bcc996c89bd55c15be876e9cc3c7738b594e8e88c14`  
		Last Modified: Fri, 11 Dec 2020 16:40:31 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:c8a1b3d790b3c92fd8f60534486432e3657290c34170182172aef7d388edf5ed
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565327785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc34adad4bc440f2db2dc13817bbfd029db0ea8e214aed77ff54bef988c690c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:44:40 GMT
ENV GOLANG_VERSION=1.14.13
# Wed, 09 Dec 2020 13:47:12 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:47:15 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:47:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:47:47 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:47:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:48:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:48:14 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e39fde14476b8b03686432399ac56cdd10a33bed19c7b6aa05a996d8053f53`  
		Last Modified: Wed, 09 Dec 2020 13:57:13 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cff7afaa3ca8e2be08888402bb3dcc49823f1b49216ea8a7db178f313b5781`  
		Last Modified: Wed, 09 Dec 2020 13:57:41 GMT  
		Size: 138.1 MB (138053353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e465bb58cd7bcb3adbbe9abeaf1f2308b5c4e96c3b616d49a93ac098014f10`  
		Last Modified: Wed, 09 Dec 2020 13:57:13 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da38c16fb5aadbc59edf287505c4b31c59e9bd51f31c5e4b3f9c1c2655b42b31`  
		Last Modified: Wed, 09 Dec 2020 22:59:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14623bec710ade7c4703d86ab2d7bc7670a2dbd62284e6a72e9293e0a1a88a3a`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e105db728228b46e8fb252863e5fcdddb822e8127e7b32e5b81e650fcce78519`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b084fc1d185874ababa327c415cacc311d3bcc66c9a692cbede771f80ba5d031`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b5cc5a51b57d325a2742d3a7b6938084fc32b1c133d582be11e204a9024d9`  
		Last Modified: Wed, 09 Dec 2020 22:59:01 GMT  
		Size: 1.8 MB (1761463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2254e03b5d914ef2fd8dc918aa9df9cb7f67c1e98a10630a2b7bb6c1f0f7f6`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:0f999aad8e883cc606f5d8beb54a02f7aaa3899a74aeef31eb5d492e548751e4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964342379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc920d3d551c5f137d1c6410054d91d0577eb8703db8237f3ee863972a2f75f1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:47:23 GMT
ENV GOLANG_VERSION=1.14.13
# Wed, 09 Dec 2020 13:50:49 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:50:51 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:48:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:48:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:48:23 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:48:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:49:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:49:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3d4eae1014fd8f0dbad49bd8a1060515845d607d2159437e80a558f2e279d`  
		Last Modified: Wed, 09 Dec 2020 13:57:54 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c045f3c54be11d4779b19209fddf2f64073ca3c46040de60f348fb3cc748ea53`  
		Last Modified: Wed, 09 Dec 2020 14:00:34 GMT  
		Size: 143.4 MB (143384254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db60e0dc4c06ac2321e7e75de87dfd689c1ad85dbaa6603fcb9273fe8936374`  
		Last Modified: Wed, 09 Dec 2020 13:57:54 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc4bad974d12e8825a23426738836e74c9e0aca1112724c1b0478bee68133c9`  
		Last Modified: Wed, 09 Dec 2020 22:59:16 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0311b51aa1cc3e230f8c7522f3f70f812ed4f8ffa261b8e837e1916458a6149`  
		Last Modified: Wed, 09 Dec 2020 22:59:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8060745a48e7df89c2f63000878e71feac7391425b2690cd93051f6aec39edcb`  
		Last Modified: Wed, 09 Dec 2020 22:59:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b0a80a94240cbcd18a1ee7e0129b89f7af1ac44d174122627211cb606fa995`  
		Last Modified: Wed, 09 Dec 2020 22:59:13 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75667bd8a8b68178e7975c90cd02492dfa3588ff239af0b3a18b1e50a27ca97`  
		Last Modified: Wed, 09 Dec 2020 22:59:17 GMT  
		Size: 11.5 MB (11464686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c091649dca72c5f08886aa6721dc558091e6659e9e0a5b13c67d448d0182f`  
		Last Modified: Wed, 09 Dec 2020 22:59:14 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-alpine`

```console
$ docker pull caddy@sha256:f12373b9a584e37a7e66eee9ae5d827d1133a8e736c6d2fbf104a218f151ea35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:37c634e75d14fc942393b95a9ca1803bc2e6eb39276cdbcb41f04653eb1aca3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120346515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3c25baf9316333b4308baa85ff5c4f5bdcdd0f2b43f480277a2427e10d43c6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:25:03 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:27:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:27:20 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:27:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:27:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:27:22 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:48:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:48:55 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:48:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:48:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:48:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:48:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff250548074e76394d085b3a57acccc88c05cbde1dbb4b27f7a7d3f752d1df0`  
		Last Modified: Fri, 04 Dec 2020 00:32:49 GMT  
		Size: 107.6 MB (107550990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c86fa391e3d32b3d1db825e61ae70f87831992751d5971c62c587526b7909cb`  
		Last Modified: Fri, 04 Dec 2020 00:32:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f309d33d760b2353f1b3cb1949ec8696c5076f42b245ae14aa1a1976fb8ab`  
		Last Modified: Fri, 04 Dec 2020 00:49:38 GMT  
		Size: 8.3 MB (8309953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a78bef7d8825ad6c9b092e9a9151f84af560335cd3492c3cd800bcf829eabda`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 1.4 MB (1407215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ee2ac4bf7c1c60fccb631b07fc1371698f356b1bf848be393ead9c77914e1`  
		Last Modified: Fri, 04 Dec 2020 00:49:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f4427023da794f7d46eef3fe23cc301a5ef9c4874e4384bbb93384d020f6f0cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115653449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6342dd6fa9a9e648434ee73c7e823cf8a90ec3c85e04666c0971fea02c6c9cf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:54 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 11 Dec 2020 05:07:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:07:42 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:07:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:07:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:07:52 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:14:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:14:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:14:33 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 08:14:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:14:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:14:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:14:40 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d14bc917e8b0e9b1e8da9e1addfea1476f1fdb73c59cfba028859bd35b6522`  
		Last Modified: Fri, 11 Dec 2020 05:09:57 GMT  
		Size: 103.5 MB (103513561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e7a785a4bea2bdefcae5d67c33482821f9fbfbad17744f3845c7fedcbf8a84`  
		Last Modified: Fri, 11 Dec 2020 05:09:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c253ffba74eeb65d966efb71aafd82bf788b9c9b9c034a1ef0ba8fd69fb89`  
		Last Modified: Fri, 11 Dec 2020 08:15:54 GMT  
		Size: 7.9 MB (7928847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5ec84babb1bb15bf1bfe449a456d7fb33928afaffe622debf4b02d9c8cb0ed`  
		Last Modified: Fri, 11 Dec 2020 08:15:53 GMT  
		Size: 1.3 MB (1327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e533154e63147025a965a7c3810aeb74085482a1424142ce76497d163a58cae`  
		Last Modified: Fri, 11 Dec 2020 08:15:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e03abef2fec55f201484597a22643a5f555b17f5bebdc057334bd7a301f424b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114812725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c2dfdfc3751b3030414e6c70bc516989641ccce757579869a633b3b31862af8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:07:09 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 00:09:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:09:40 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:09:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:09:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:09:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:05 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 00:33:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc832c4959c984d61cbf9ca04945922a7ac84d32c9a7dbfc4000f56b593f8fe`  
		Last Modified: Fri, 04 Dec 2020 00:16:33 GMT  
		Size: 103.7 MB (103655540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75782af3feb5c44682b68de6dbe1678c0028b8316b235c6bb325c9b96d47466f`  
		Last Modified: Fri, 04 Dec 2020 00:15:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3103923df4c137961411ee9beb2163bb0fceb96024cab996b338fff9dec323cb`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 7.1 MB (7144867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267c9a980b43f5e19848c54b902901643b512e49bca7eeb2694d6395d58d9e5`  
		Last Modified: Fri, 04 Dec 2020 00:33:59 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95b1cb145016023a360ff49d799308bb9a33fdaa990f076ead6e8454424856e`  
		Last Modified: Fri, 04 Dec 2020 00:33:58 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c342415c2eacab2e75ff361dc7a30271d8693f36dfa5812bc9a73b45fb7650e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115766627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26fb7973448a7a127743363016ea1407c9372ff89327d196152ccb285a64d74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:02:52 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 01:04:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:04:52 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:04:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:04:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:04:56 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:07 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:08 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 01:28:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:13 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f038c27fba9771a10e2d17f066f31884e1d64e9d50f996d4e1f98c7d9eca6df5`  
		Last Modified: Fri, 04 Dec 2020 01:11:44 GMT  
		Size: 103.0 MB (102968080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb141fcf8afeddffe403b798e502235e8746a2bbcecb5325ae2067d6e64aedc`  
		Last Modified: Fri, 04 Dec 2020 01:11:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237402524d7a7d687e3e2866ec83f21ad5a498ed7f26f1a8236cda6b5f560929`  
		Last Modified: Fri, 04 Dec 2020 01:28:54 GMT  
		Size: 8.5 MB (8499866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c71374c7630456a387209dca122b16a8038192403356b827b0dfa2ab77eff`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 1.3 MB (1310182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6da552cad766345c3058306ad61d20a6f02651f46d71ce40583fc9f18762f7`  
		Last Modified: Fri, 04 Dec 2020 01:28:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:a3966dfa7df24217bd14943995fc0e4d6d8084992a5c389ccbca4f4118804b22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115150516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef65b689756199e63647a98cebfe48993694a73b122f91d3be33a2d69ce7c56`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:59:55 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 04 Dec 2020 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 02:02:08 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 02:02:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 02:02:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 02:02:24 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:12:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:12:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:12:34 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 04 Dec 2020 03:12:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:12:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:12:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f63d5e2daabbfe6e2070563b812f7d8cedf414d153c493cd60bfc611e364dc9`  
		Last Modified: Fri, 04 Dec 2020 02:08:29 GMT  
		Size: 101.9 MB (101855605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07277d6b2e6785d1fc5318d4c63b413a76cb86a9d7beeb0d20bdd835d34eea19`  
		Last Modified: Fri, 04 Dec 2020 02:08:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6e1068327176aa38aa1e6a20aa01eeeb3b9427cbc0f41fbe367cc06474325b`  
		Last Modified: Fri, 04 Dec 2020 03:14:31 GMT  
		Size: 8.9 MB (8919981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86508b35ca9f1a8e0db3f8fc347a62e1e17b591a7785c85705169631d0df17d1`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50938474f3e06598b1f0264f5bc734dde207d35f09f032ddae0bcf66fe7252e2`  
		Last Modified: Fri, 04 Dec 2020 03:14:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:eb0a6338a700322a20d0aa43f2806d21e393e6ea8223c279d2478aac22c2def6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.7 MB (119651264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2693c682f63cd6fcfd6ed02092b945cea78feada8d46df763f09b96776c21818`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:30 GMT
ENV GOLANG_VERSION=1.14.13
# Fri, 11 Dec 2020 03:34:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.13.src.tar.gz'; 	sha256='ba1d244c6b5c0ed04aa0d7856d06aceb89ed31b895de6ff783efb1cc8ab6b177'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:34:24 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:34:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:34:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:36 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:36 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 11 Dec 2020 16:39:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:40 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cad920206526b07e54157f3f3e750c020714ef2fa81afaf15795a370a17c16d`  
		Last Modified: Fri, 11 Dec 2020 03:35:53 GMT  
		Size: 107.1 MB (107062213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4289f50a1bbc5253453a64e5de3e8ea337aaac81e21fcef64eeeaea68d0e507`  
		Last Modified: Fri, 11 Dec 2020 03:35:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7067c7cd350e8ef505f157b1add8a9a301c34ef4504b86eeba9d327253e4c55`  
		Last Modified: Fri, 11 Dec 2020 16:40:32 GMT  
		Size: 8.4 MB (8352271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23965c15ee31da004d6acd1aeed41b837d70bb87a1240266dd2ccc6b1722f7ee`  
		Last Modified: Fri, 11 Dec 2020 16:40:33 GMT  
		Size: 1.4 MB (1388754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dccb0aaab794fa2f8fd0bcc996c89bd55c15be876e9cc3c7738b594e8e88c14`  
		Last Modified: Fri, 11 Dec 2020 16:40:31 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:599455209c356e28c81d243ab04bafbf12cb8c5692a01b9667f6db19b56b27c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:2.1.1-builder-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:c8a1b3d790b3c92fd8f60534486432e3657290c34170182172aef7d388edf5ed
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565327785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc34adad4bc440f2db2dc13817bbfd029db0ea8e214aed77ff54bef988c690c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:44:40 GMT
ENV GOLANG_VERSION=1.14.13
# Wed, 09 Dec 2020 13:47:12 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:47:15 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:47:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:47:47 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:47:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:48:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:48:14 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e39fde14476b8b03686432399ac56cdd10a33bed19c7b6aa05a996d8053f53`  
		Last Modified: Wed, 09 Dec 2020 13:57:13 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cff7afaa3ca8e2be08888402bb3dcc49823f1b49216ea8a7db178f313b5781`  
		Last Modified: Wed, 09 Dec 2020 13:57:41 GMT  
		Size: 138.1 MB (138053353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e465bb58cd7bcb3adbbe9abeaf1f2308b5c4e96c3b616d49a93ac098014f10`  
		Last Modified: Wed, 09 Dec 2020 13:57:13 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da38c16fb5aadbc59edf287505c4b31c59e9bd51f31c5e4b3f9c1c2655b42b31`  
		Last Modified: Wed, 09 Dec 2020 22:59:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14623bec710ade7c4703d86ab2d7bc7670a2dbd62284e6a72e9293e0a1a88a3a`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e105db728228b46e8fb252863e5fcdddb822e8127e7b32e5b81e650fcce78519`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b084fc1d185874ababa327c415cacc311d3bcc66c9a692cbede771f80ba5d031`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b5cc5a51b57d325a2742d3a7b6938084fc32b1c133d582be11e204a9024d9`  
		Last Modified: Wed, 09 Dec 2020 22:59:01 GMT  
		Size: 1.8 MB (1761463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2254e03b5d914ef2fd8dc918aa9df9cb7f67c1e98a10630a2b7bb6c1f0f7f6`  
		Last Modified: Wed, 09 Dec 2020 22:58:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9b8a62d75220bf229866859c752c8270f53e452bcba9ec1325af307115fd9da5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.1.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:0f999aad8e883cc606f5d8beb54a02f7aaa3899a74aeef31eb5d492e548751e4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964342379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc920d3d551c5f137d1c6410054d91d0577eb8703db8237f3ee863972a2f75f1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:47:23 GMT
ENV GOLANG_VERSION=1.14.13
# Wed, 09 Dec 2020 13:50:49 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '18c5597d7648ce3872f4a0a7bc73a70c01b56b77feac5e5f80b2ecba0d231473'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:50:51 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:48:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:48:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:48:23 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:48:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:49:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:49:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3d4eae1014fd8f0dbad49bd8a1060515845d607d2159437e80a558f2e279d`  
		Last Modified: Wed, 09 Dec 2020 13:57:54 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c045f3c54be11d4779b19209fddf2f64073ca3c46040de60f348fb3cc748ea53`  
		Last Modified: Wed, 09 Dec 2020 14:00:34 GMT  
		Size: 143.4 MB (143384254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db60e0dc4c06ac2321e7e75de87dfd689c1ad85dbaa6603fcb9273fe8936374`  
		Last Modified: Wed, 09 Dec 2020 13:57:54 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc4bad974d12e8825a23426738836e74c9e0aca1112724c1b0478bee68133c9`  
		Last Modified: Wed, 09 Dec 2020 22:59:16 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0311b51aa1cc3e230f8c7522f3f70f812ed4f8ffa261b8e837e1916458a6149`  
		Last Modified: Wed, 09 Dec 2020 22:59:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8060745a48e7df89c2f63000878e71feac7391425b2690cd93051f6aec39edcb`  
		Last Modified: Wed, 09 Dec 2020 22:59:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b0a80a94240cbcd18a1ee7e0129b89f7af1ac44d174122627211cb606fa995`  
		Last Modified: Wed, 09 Dec 2020 22:59:13 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75667bd8a8b68178e7975c90cd02492dfa3588ff239af0b3a18b1e50a27ca97`  
		Last Modified: Wed, 09 Dec 2020 22:59:17 GMT  
		Size: 11.5 MB (11464686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c091649dca72c5f08886aa6721dc558091e6659e9e0a5b13c67d448d0182f`  
		Last Modified: Wed, 09 Dec 2020 22:59:14 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:45aabf65811a78879dbfae6b00bfcd8778127d1b97dc2c54ec41276d96162ff8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:9a3bcc6076982ff8b0833a250a3bdec2f0fc180d3869a50df2c5111c35900756
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2418118741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eabf81561f405d4bdf2b4704d6ca869edc7ddea014dd1abe0f360edb2f249ed6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:42:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:42:47 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:43:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:43:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:43:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:43:23 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:43:24 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:43:24 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Dec 2020 22:43:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:43:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:43:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:43:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:43:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:43:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:43:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:43:30 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:43:31 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:43:31 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:43:47 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:43:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8310e6a3befeed4407572cd52b3887e0fda9b586ca388d76f9e9e14f0174d6`  
		Last Modified: Wed, 09 Dec 2020 22:58:23 GMT  
		Size: 9.2 MB (9243060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e21e51fee4a54f410d2f26105f8ee67030de4d0c2f7e977ac39a5635f093c5`  
		Last Modified: Wed, 09 Dec 2020 22:58:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24348cbc7752073f17d52670e5f5678337f4f518ae178cc70a98daaab1b3b4`  
		Last Modified: Wed, 09 Dec 2020 22:58:24 GMT  
		Size: 17.7 MB (17701596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6652d297bd09a384ff9270741baf15f8273217c718aae1a2b722fde0354fab17`  
		Last Modified: Wed, 09 Dec 2020 22:58:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f68b024395847bee888c4527f15e46931af7c4b33eba653fe6b3e5f91d90bf`  
		Last Modified: Wed, 09 Dec 2020 22:58:18 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5c45ff80ddf22adcfc93ef960cbc1fb6389e7b836abb8a29ec0fed22ac25`  
		Last Modified: Wed, 09 Dec 2020 22:58:17 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92e3d73352785cfd5be7f16932b53670b41691d227980cd835bf418f14d8a82`  
		Last Modified: Wed, 09 Dec 2020 22:58:17 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6f5bbdfb82b660d77e1075f9af7110b7bfe9f6708c60f15f8aa2df164b45ee`  
		Last Modified: Wed, 09 Dec 2020 22:58:16 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974f29c0c664d8a7edccac5aea85146f0c28f08450b89315bac02e12bcb803c`  
		Last Modified: Wed, 09 Dec 2020 22:58:16 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7a2fbf68d6d2c48d7221407dbf9de908850675adef8e05da13dcfdd889f2b1`  
		Last Modified: Wed, 09 Dec 2020 22:58:15 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab33f16822bafab6e4e5d8cb0239224fa9ded2b36ab1f043c58ee1090ffffe5b`  
		Last Modified: Wed, 09 Dec 2020 22:58:13 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b973cee99b817a2b430e8b288d5bbf5345a86c7a8bc7478db3bb7a06fc8a08f`  
		Last Modified: Wed, 09 Dec 2020 22:58:14 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f9be9ebe03c3c6264d1187eb40cf64cb2e3a0797b9c7d7020fe89e7446b3`  
		Last Modified: Wed, 09 Dec 2020 22:58:14 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f928962368a43603f41dd1b4d7cc013507a02b94a0c04b895f9b36a95b2d69`  
		Last Modified: Wed, 09 Dec 2020 22:58:13 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266811a4d21e656edad5a4620f4665d9af80a27efcf1939e3e421f9dc5be643`  
		Last Modified: Wed, 09 Dec 2020 22:58:12 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06371064917888a8d76cf047c3d638ab2c47c1d1455af625e5328dfe7ccd9106`  
		Last Modified: Wed, 09 Dec 2020 22:58:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeb1400c5654b601c27186e5d01a98b7edac4e1eab9e685a72a5b76e051b649`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643137612c3791ba413e0c82a6ab3a7bfc9e0f63d12606aa5100a601e5537867`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ebbab633b643578785da16143e2bea1a1e3a0a084a69bc3926b7874f6f0b4`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 279.1 KB (279142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec87bc08f9747fe4d23aa34857acb63e17bfb53f1c218b84c375528171675bc`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:bef89cd4397dfc72efac26c3af66c367167de1f7beb5fa15b9eb16103d69edfd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802183304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27357e1c65458f12556946c0756fa611e58dd1e58fce5e1d3c744cfc6ad3d26d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:45:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:45:21 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:46:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:46:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:46:47 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:46:48 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:46:49 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:46:50 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Dec 2020 22:46:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:46:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:46:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:46:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:46:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:46:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:46:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:46:56 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:46:57 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:46:57 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:47:41 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:47:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb3365d5b5f52406d1460ea71ec7dc45a0be84fb11ee92a095c01446982ac`  
		Last Modified: Wed, 09 Dec 2020 22:58:47 GMT  
		Size: 10.1 MB (10058753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7e40284fe73310de6916db9588492c76d9faf162ba20cc75e06f28cdf5b5d3`  
		Last Modified: Wed, 09 Dec 2020 22:58:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d808c13287b5d9fe34c6cc197e3a5f1c625583988ab9261ad38969f3b3bb727`  
		Last Modified: Wed, 09 Dec 2020 22:58:49 GMT  
		Size: 23.0 MB (23021357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0327ccf8c96f9c862dcbb6a7b88a7834597610a976c6a1a0e5b6e60705337019`  
		Last Modified: Wed, 09 Dec 2020 22:58:42 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45aa920e303bd017aa55620871520648cd55969ae89963b8180cf8462a06d9f`  
		Last Modified: Wed, 09 Dec 2020 22:58:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06dc416d5acc13c105dfb12dc601bf956d10efef6ef96d5639fdba94d236762`  
		Last Modified: Wed, 09 Dec 2020 22:58:41 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad9f0882cad71b6b14c48e7ffa0ca9b90bb89d577097f1cb2f7892cb1fcb780`  
		Last Modified: Wed, 09 Dec 2020 22:58:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e4736002f89abfa7f6da14661a1f6a4d2ae079c3f31102bffe18cdd8beeb6d`  
		Last Modified: Wed, 09 Dec 2020 22:58:39 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86169177264c9317107ac0a5ca73674c2de958677546206af268ee1f54dd084`  
		Last Modified: Wed, 09 Dec 2020 22:58:39 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5448bd5ec4e8f017b5a6ad026679927adffa04f4cad61f078dad05f5698afd`  
		Last Modified: Wed, 09 Dec 2020 22:58:38 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fc40c7d9ddfd83bff64476793cb83f8f16c29f719ef4ac1ab472ccfd21527a`  
		Last Modified: Wed, 09 Dec 2020 22:58:37 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69dd9ca0f7b2f5dcd5a208296f33e5b2e918b471971464afecaea0528dca320`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1467e2c551c61df53878d778d60d4206f2b0985166be921d43025fe9eea9a617`  
		Last Modified: Wed, 09 Dec 2020 22:58:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ffdf83969e06a380e2e5ad6d6e247cecf5ab242f9388917e95c3cb442a087`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb4589051190d97302d6ec12f716820272f7c07dac4e4a3cf2685ec1d4404c`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb4bdcb4f4f977edee7bd1de9042084c67eb27db3c8a820f6e463da7c6198e9`  
		Last Modified: Wed, 09 Dec 2020 22:58:33 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bec2c9e631017e4bd85ef16b73b059ae9dcd2d65e96093e91332872b4a484d`  
		Last Modified: Wed, 09 Dec 2020 22:58:33 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdf38a5e62965ddd16e787d39db0033eec3827e459ed8c8b8edd00b2742ba3d`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf1879d55948e8a6692625974f1ce349eb596a2ee5fae7442503b720ffe6768`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 238.7 KB (238665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79a4b2f0acee85ce6edc7959ba4733df596c028ad2e07d6626581d716531869`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:98b234573081604efc7741c99c8755560ecc70d5f3bf02bf063b2b939e88ac03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:9a3bcc6076982ff8b0833a250a3bdec2f0fc180d3869a50df2c5111c35900756
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2418118741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eabf81561f405d4bdf2b4704d6ca869edc7ddea014dd1abe0f360edb2f249ed6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:42:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:42:47 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:43:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:43:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:43:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:43:23 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:43:24 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:43:24 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Dec 2020 22:43:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:43:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:43:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:43:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:43:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:43:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:43:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:43:30 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:43:31 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:43:31 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:43:47 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:43:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8310e6a3befeed4407572cd52b3887e0fda9b586ca388d76f9e9e14f0174d6`  
		Last Modified: Wed, 09 Dec 2020 22:58:23 GMT  
		Size: 9.2 MB (9243060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e21e51fee4a54f410d2f26105f8ee67030de4d0c2f7e977ac39a5635f093c5`  
		Last Modified: Wed, 09 Dec 2020 22:58:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24348cbc7752073f17d52670e5f5678337f4f518ae178cc70a98daaab1b3b4`  
		Last Modified: Wed, 09 Dec 2020 22:58:24 GMT  
		Size: 17.7 MB (17701596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6652d297bd09a384ff9270741baf15f8273217c718aae1a2b722fde0354fab17`  
		Last Modified: Wed, 09 Dec 2020 22:58:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f68b024395847bee888c4527f15e46931af7c4b33eba653fe6b3e5f91d90bf`  
		Last Modified: Wed, 09 Dec 2020 22:58:18 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35af5c45ff80ddf22adcfc93ef960cbc1fb6389e7b836abb8a29ec0fed22ac25`  
		Last Modified: Wed, 09 Dec 2020 22:58:17 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92e3d73352785cfd5be7f16932b53670b41691d227980cd835bf418f14d8a82`  
		Last Modified: Wed, 09 Dec 2020 22:58:17 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6f5bbdfb82b660d77e1075f9af7110b7bfe9f6708c60f15f8aa2df164b45ee`  
		Last Modified: Wed, 09 Dec 2020 22:58:16 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974f29c0c664d8a7edccac5aea85146f0c28f08450b89315bac02e12bcb803c`  
		Last Modified: Wed, 09 Dec 2020 22:58:16 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7a2fbf68d6d2c48d7221407dbf9de908850675adef8e05da13dcfdd889f2b1`  
		Last Modified: Wed, 09 Dec 2020 22:58:15 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab33f16822bafab6e4e5d8cb0239224fa9ded2b36ab1f043c58ee1090ffffe5b`  
		Last Modified: Wed, 09 Dec 2020 22:58:13 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b973cee99b817a2b430e8b288d5bbf5345a86c7a8bc7478db3bb7a06fc8a08f`  
		Last Modified: Wed, 09 Dec 2020 22:58:14 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d0f9be9ebe03c3c6264d1187eb40cf64cb2e3a0797b9c7d7020fe89e7446b3`  
		Last Modified: Wed, 09 Dec 2020 22:58:14 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f928962368a43603f41dd1b4d7cc013507a02b94a0c04b895f9b36a95b2d69`  
		Last Modified: Wed, 09 Dec 2020 22:58:13 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266811a4d21e656edad5a4620f4665d9af80a27efcf1939e3e421f9dc5be643`  
		Last Modified: Wed, 09 Dec 2020 22:58:12 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06371064917888a8d76cf047c3d638ab2c47c1d1455af625e5328dfe7ccd9106`  
		Last Modified: Wed, 09 Dec 2020 22:58:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeb1400c5654b601c27186e5d01a98b7edac4e1eab9e685a72a5b76e051b649`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643137612c3791ba413e0c82a6ab3a7bfc9e0f63d12606aa5100a601e5537867`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ebbab633b643578785da16143e2bea1a1e3a0a084a69bc3926b7874f6f0b4`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 279.1 KB (279142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec87bc08f9747fe4d23aa34857acb63e17bfb53f1c218b84c375528171675bc`  
		Last Modified: Wed, 09 Dec 2020 22:58:09 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:8dfddeecaaab0f6038dd9ca21ace1057891ceb45831f4f9f76211c9800192ea0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:bef89cd4397dfc72efac26c3af66c367167de1f7beb5fa15b9eb16103d69edfd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802183304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27357e1c65458f12556946c0756fa611e58dd1e58fce5e1d3c744cfc6ad3d26d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:45:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:45:21 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Dec 2020 22:46:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:46:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:46:47 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:46:48 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:46:49 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:46:50 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Dec 2020 22:46:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:46:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:46:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:46:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:46:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:46:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:46:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:46:56 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:46:57 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:46:57 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:47:41 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:47:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb3365d5b5f52406d1460ea71ec7dc45a0be84fb11ee92a095c01446982ac`  
		Last Modified: Wed, 09 Dec 2020 22:58:47 GMT  
		Size: 10.1 MB (10058753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7e40284fe73310de6916db9588492c76d9faf162ba20cc75e06f28cdf5b5d3`  
		Last Modified: Wed, 09 Dec 2020 22:58:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d808c13287b5d9fe34c6cc197e3a5f1c625583988ab9261ad38969f3b3bb727`  
		Last Modified: Wed, 09 Dec 2020 22:58:49 GMT  
		Size: 23.0 MB (23021357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0327ccf8c96f9c862dcbb6a7b88a7834597610a976c6a1a0e5b6e60705337019`  
		Last Modified: Wed, 09 Dec 2020 22:58:42 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45aa920e303bd017aa55620871520648cd55969ae89963b8180cf8462a06d9f`  
		Last Modified: Wed, 09 Dec 2020 22:58:41 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06dc416d5acc13c105dfb12dc601bf956d10efef6ef96d5639fdba94d236762`  
		Last Modified: Wed, 09 Dec 2020 22:58:41 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad9f0882cad71b6b14c48e7ffa0ca9b90bb89d577097f1cb2f7892cb1fcb780`  
		Last Modified: Wed, 09 Dec 2020 22:58:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e4736002f89abfa7f6da14661a1f6a4d2ae079c3f31102bffe18cdd8beeb6d`  
		Last Modified: Wed, 09 Dec 2020 22:58:39 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86169177264c9317107ac0a5ca73674c2de958677546206af268ee1f54dd084`  
		Last Modified: Wed, 09 Dec 2020 22:58:39 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5448bd5ec4e8f017b5a6ad026679927adffa04f4cad61f078dad05f5698afd`  
		Last Modified: Wed, 09 Dec 2020 22:58:38 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fc40c7d9ddfd83bff64476793cb83f8f16c29f719ef4ac1ab472ccfd21527a`  
		Last Modified: Wed, 09 Dec 2020 22:58:37 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69dd9ca0f7b2f5dcd5a208296f33e5b2e918b471971464afecaea0528dca320`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1467e2c551c61df53878d778d60d4206f2b0985166be921d43025fe9eea9a617`  
		Last Modified: Wed, 09 Dec 2020 22:58:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ffdf83969e06a380e2e5ad6d6e247cecf5ab242f9388917e95c3cb442a087`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb4589051190d97302d6ec12f716820272f7c07dac4e4a3cf2685ec1d4404c`  
		Last Modified: Wed, 09 Dec 2020 22:58:36 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb4bdcb4f4f977edee7bd1de9042084c67eb27db3c8a820f6e463da7c6198e9`  
		Last Modified: Wed, 09 Dec 2020 22:58:33 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bec2c9e631017e4bd85ef16b73b059ae9dcd2d65e96093e91332872b4a484d`  
		Last Modified: Wed, 09 Dec 2020 22:58:33 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdf38a5e62965ddd16e787d39db0033eec3827e459ed8c8b8edd00b2742ba3d`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf1879d55948e8a6692625974f1ce349eb596a2ee5fae7442503b720ffe6768`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 238.7 KB (238665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79a4b2f0acee85ce6edc7959ba4733df596c028ad2e07d6626581d716531869`  
		Last Modified: Wed, 09 Dec 2020 22:58:34 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1`

```console
$ docker pull caddy@sha256:3bdc57eb2bf54c1df10c43fc566f1cc5269f6ae8a5b9a86e3b9fa98a614a66d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.2.1` - linux; amd64

```console
$ docker pull caddy@sha256:5c14834055e3ec0800789a46db92258f78556ef9971457022234e3487c2ae207
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4daabe9339412068d7bcc4c9b0ac275c67c82d8c819e4b37a387b50fa8e9a61b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:28:21 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:28 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4428f13c7edb68201eb53fc2a833e3e1831b1bfc66d8ca591d7d7981e8dcdb57`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b931870cc5c313c5b12bd911762577180c41684025e803ac19870628f24474`  
		Last Modified: Fri, 11 Dec 2020 02:29:11 GMT  
		Size: 11.5 MB (11532507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010bdd923cf20d340b6e9f06cac8c3f1e1984172c4f4d095cd9b443b03ad818`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ee965d543057e5cb4af597d364066251a9852583059cd38488243306b724a778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7753d72769487802d1fee3d3f07ee3ce735418d63d93259ad8125a3ae2de1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:10:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:10:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:10:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:10:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:10:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:10:21 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:10:21 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:10:22 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:10:23 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:10:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:10:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:10:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:10:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:10:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:10:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:10:31 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:10:32 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:10:33 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:10:35 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:10:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7ab50db8ca6e467811f1281518708c79ffb3eba857ede634fe075aa109cf4`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c5497e98ba2efc52fb51339d08617c1ffc210163f8774632f307c81683deb`  
		Last Modified: Fri, 11 Dec 2020 03:11:27 GMT  
		Size: 10.9 MB (10876275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140a3a819ce00971b2089202730b7c285ca9a6ab1f5832820b20a043fd51fcc9`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2d82fb7e660d56846fa3c33deb953bfc6c464bfb8fba608c237b4a5e0eee33c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e57be32d04a04308b9f9c3fcbac701e798783ecbe10f243a411262f5a05cb0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:07:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:07:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:07:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:07:14 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:07:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:07:16 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:07:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:07:18 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:07:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:07:24 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:07:25 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:07:26 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:07:27 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:07:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2348443ed0fb4b09e2d5b6d636d90e4bbf2024e934143fadfcc35bbc65a709a1`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8462380e6876aca9643bcf369ffc7b958a08c3fd3fc56a861ca651a1fcaf9c`  
		Last Modified: Fri, 11 Dec 2020 03:08:19 GMT  
		Size: 10.9 MB (10854381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7839ddc84cd5ea73da141c2726d80c7493a37772c128eb7f60b1621784acf0`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8a8a108facaeb348bc873b80764a0e142fa06279dce55fc16f6d68017de99f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b781915644b6cb14f7dbcb44242df9845f6f989c96c3b75da745a4c11d116ca0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:33:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:33:42 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:33:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:33:52 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:33:53 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:34:00 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:34:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:34:03 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:34:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:34:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:34:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:34:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:34:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:34:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:34:19 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:34:21 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:34:23 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:34:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a6157741b4baecc6781d3a2227bd753df1a152366cfba7d5f83731611b38f3`  
		Last Modified: Fri, 11 Dec 2020 03:35:17 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f6d968230fb7b05d7bb6b35f8eab026c6e68c93458a9c40095b9bccb7eb23d`  
		Last Modified: Fri, 11 Dec 2020 03:35:20 GMT  
		Size: 10.5 MB (10527460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665b752f90ad5d8f5f8c6840c5cc58eb1b542c21773b827303c156732f73321`  
		Last Modified: Fri, 11 Dec 2020 03:35:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:b5c5d0c317892db3c940899c940405ad1283f0857b3cb1c454abce45a325b8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf8c3b1e29b5c01bce118fbc104af2924a4b50324db40dedeb78ba2d9df4c33`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 06:44:22 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 06:44:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:44:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:44:48 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:44:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:44:54 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:44:57 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:45:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 06:45:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:45:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:45:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:45:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:45:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:45:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:45:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:45:35 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:45:39 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:45:45 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:45:49 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:45:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f10029b2ed0c8a52065e9b56b5b27d4f7a83fcba0392c7021532236b70a0f`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd4c79b504a226097858b4a8bc37dbed1031f3a3205cf552a5ebceb132f791`  
		Last Modified: Fri, 11 Dec 2020 06:46:51 GMT  
		Size: 10.2 MB (10180214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2cc34795b6c9d9081692bd53a1f7b77ae6a7c9e9e661f863cc493d6973a26`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; s390x

```console
$ docker pull caddy@sha256:90b5dcd8d713f82a46c2039baee451f911f8d25f27431e6b44655f8b2803c557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f49a1c397b4a9cdc0f9a6cd1eb6aea12154952a3d4ead09ddd6c9595bb4361`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:43:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:43:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:50 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752f95e37b35ec8cf81bd3caab7ba2ea836620747fa2d720c5b64709254ddae`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f574024c894c439da18a68fa9e20ef03be94dd77a2b1934242463f93d518b0`  
		Last Modified: Fri, 11 Dec 2020 02:44:34 GMT  
		Size: 11.2 MB (11202556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26947b55683beda16dec6f01fc3ef037d91c61349dae0527952bafce3c03d5c0`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-alpine`

```console
$ docker pull caddy@sha256:a4d99ca9d9c9c0b2c8bd2ffe356ed4ca5e0ebe5141a09af64b5ff72a71f7d72f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:5c14834055e3ec0800789a46db92258f78556ef9971457022234e3487c2ae207
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4daabe9339412068d7bcc4c9b0ac275c67c82d8c819e4b37a387b50fa8e9a61b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:28:21 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:28 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4428f13c7edb68201eb53fc2a833e3e1831b1bfc66d8ca591d7d7981e8dcdb57`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b931870cc5c313c5b12bd911762577180c41684025e803ac19870628f24474`  
		Last Modified: Fri, 11 Dec 2020 02:29:11 GMT  
		Size: 11.5 MB (11532507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010bdd923cf20d340b6e9f06cac8c3f1e1984172c4f4d095cd9b443b03ad818`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ee965d543057e5cb4af597d364066251a9852583059cd38488243306b724a778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7753d72769487802d1fee3d3f07ee3ce735418d63d93259ad8125a3ae2de1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:10:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:10:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:10:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:10:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:10:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:10:21 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:10:21 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:10:22 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:10:23 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:10:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:10:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:10:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:10:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:10:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:10:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:10:31 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:10:32 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:10:33 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:10:35 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:10:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7ab50db8ca6e467811f1281518708c79ffb3eba857ede634fe075aa109cf4`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c5497e98ba2efc52fb51339d08617c1ffc210163f8774632f307c81683deb`  
		Last Modified: Fri, 11 Dec 2020 03:11:27 GMT  
		Size: 10.9 MB (10876275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140a3a819ce00971b2089202730b7c285ca9a6ab1f5832820b20a043fd51fcc9`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2d82fb7e660d56846fa3c33deb953bfc6c464bfb8fba608c237b4a5e0eee33c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e57be32d04a04308b9f9c3fcbac701e798783ecbe10f243a411262f5a05cb0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:07:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:07:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:07:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:07:14 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:07:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:07:16 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:07:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:07:18 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:07:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:07:24 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:07:25 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:07:26 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:07:27 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:07:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2348443ed0fb4b09e2d5b6d636d90e4bbf2024e934143fadfcc35bbc65a709a1`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8462380e6876aca9643bcf369ffc7b958a08c3fd3fc56a861ca651a1fcaf9c`  
		Last Modified: Fri, 11 Dec 2020 03:08:19 GMT  
		Size: 10.9 MB (10854381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7839ddc84cd5ea73da141c2726d80c7493a37772c128eb7f60b1621784acf0`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8a8a108facaeb348bc873b80764a0e142fa06279dce55fc16f6d68017de99f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b781915644b6cb14f7dbcb44242df9845f6f989c96c3b75da745a4c11d116ca0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:33:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:33:42 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:33:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:33:52 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:33:53 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:34:00 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:34:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:34:03 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:34:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:34:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:34:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:34:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:34:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:34:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:34:19 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:34:21 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:34:23 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:34:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a6157741b4baecc6781d3a2227bd753df1a152366cfba7d5f83731611b38f3`  
		Last Modified: Fri, 11 Dec 2020 03:35:17 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f6d968230fb7b05d7bb6b35f8eab026c6e68c93458a9c40095b9bccb7eb23d`  
		Last Modified: Fri, 11 Dec 2020 03:35:20 GMT  
		Size: 10.5 MB (10527460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665b752f90ad5d8f5f8c6840c5cc58eb1b542c21773b827303c156732f73321`  
		Last Modified: Fri, 11 Dec 2020 03:35:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b5c5d0c317892db3c940899c940405ad1283f0857b3cb1c454abce45a325b8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf8c3b1e29b5c01bce118fbc104af2924a4b50324db40dedeb78ba2d9df4c33`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 06:44:22 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 06:44:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:44:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:44:48 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:44:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:44:54 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:44:57 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:45:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 06:45:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:45:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:45:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:45:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:45:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:45:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:45:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:45:35 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:45:39 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:45:45 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:45:49 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:45:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f10029b2ed0c8a52065e9b56b5b27d4f7a83fcba0392c7021532236b70a0f`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd4c79b504a226097858b4a8bc37dbed1031f3a3205cf552a5ebceb132f791`  
		Last Modified: Fri, 11 Dec 2020 06:46:51 GMT  
		Size: 10.2 MB (10180214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2cc34795b6c9d9081692bd53a1f7b77ae6a7c9e9e661f863cc493d6973a26`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:90b5dcd8d713f82a46c2039baee451f911f8d25f27431e6b44655f8b2803c557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f49a1c397b4a9cdc0f9a6cd1eb6aea12154952a3d4ead09ddd6c9595bb4361`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:43:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:43:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:50 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752f95e37b35ec8cf81bd3caab7ba2ea836620747fa2d720c5b64709254ddae`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f574024c894c439da18a68fa9e20ef03be94dd77a2b1934242463f93d518b0`  
		Last Modified: Fri, 11 Dec 2020 02:44:34 GMT  
		Size: 11.2 MB (11202556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26947b55683beda16dec6f01fc3ef037d91c61349dae0527952bafce3c03d5c0`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder`

```console
$ docker pull caddy@sha256:f6c2dae67ff30eb30043f191a9666b390ade3f947c76c2d4f1e917ccd3767f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.2.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:5dd4797c97ea381ace1e1eea532fd5f29423ac06b12c619cafe000d64509feb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114700864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7df7c6f834dd58c1afbd8a64abe410fc1e80ec544708fa9a965f57ab86a1d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:15:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:15:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:15:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 08:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:15:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:15:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:15:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf7daeb76c3bb0b9919f840ee1313d7bf03e238f25ccfa50685ba22c0a0948`  
		Last Modified: Fri, 11 Dec 2020 08:16:06 GMT  
		Size: 7.9 MB (7928844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b6373b354ba393226a1d7e15beb5d3919235aebaad2e462b77a90718b558e`  
		Last Modified: Fri, 11 Dec 2020 08:16:04 GMT  
		Size: 1.3 MB (1327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1a1637bd896f4e26717e8304024ce908354fa2dc98efa5cc9f259041d9e42`  
		Last Modified: Fri, 11 Dec 2020 08:16:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:d4ebeec4a896b43b05053e5f61d4d78aebf77717043d77fcae5f8b903ad10631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118414315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3467a549ea0fdd27eab9873a3dc66116f589f7fb59ddfcfce4d3e0754b62f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:55 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 16:39:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433be6df8d40c95a43238d4562dc038798dbafe8378275ac6f7892c47c2556d`  
		Last Modified: Fri, 11 Dec 2020 16:40:50 GMT  
		Size: 8.4 MB (8352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bae692d5a8f8b212bd467f34afe61584d54eb7761d05104582b79fa0590a52f`  
		Last Modified: Fri, 11 Dec 2020 16:40:48 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64532095c920265ad0fe12449c16c4c91e2f65d579d594917175d9b0f79e71bd`  
		Last Modified: Fri, 11 Dec 2020 16:40:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:243fdb842eb0ae5c699a0b2c6b21e073188b55d46b5f1676019f0f095ffca10f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565628646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba058fb2a4eb196ac68f44e313a930f00c616e461f23e6bfa1edf451b3b3bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:55:28 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:55:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:55:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:55:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206310242577d11bd5feb3aa11b5f7d090a6edc146c4b229e6a4975cf73c1286`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903040d044b4614ed82d2ea5c95b10d236be0d4e4663b746f0c926fec5da92f`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0805737182f599ffeb040b6aa7f9338886390514b97d8ad6a9d020416344b`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad7c66c28d14e3a2438621bd6ce3eb16838bc04cec4e38be4022719b6b2ec9`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123020c4e3f3f7ca21810e8fbd2ce260e1962aa76fe2ddef3044a6e7614a10f8`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.8 MB (1761375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85eee7c96161123b7862f2e6ef2594e84968b082fd7f819a0c26ed08d476a30`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:b75948041fc580c0d1edd8aa722a8277bb301ba41d8b590a4f17c66c9fe4ab40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964606778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a2250a1f590dde32f7e679b96a04ed050c4655a60ae952af73b0c26d598c80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:59 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:56:00 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:56:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:57:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:57:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4e04e74a87b1fb4ec35b081bb61d4e85f9f0b3a80c88d8a44a20efc94584e`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342b3373ee29de0d987f0b40171c41395e9b00269cab4de6dbf2a90503cef74`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973292c9e2947dc0e10764597f6f9f50d9e521151f3f1ffce12110bd59d7ac9`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeda6d1d0446d45cf769ad800da810928a915a53f0f15741d1f2d5e330bfbd`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03028d69a4efd9fca773e4c828323c76cc768d9f5842bff350846206e20642c6`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 11.5 MB (11462074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5c946ea76708b5d1b6c1393f0d926d12c16e5eac35699436370388d806e55`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-alpine`

```console
$ docker pull caddy@sha256:a0597f0650078a269e9d2c9b1e69bf3a13e695884ee2a9342df0d860d6b5e3a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:5dd4797c97ea381ace1e1eea532fd5f29423ac06b12c619cafe000d64509feb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114700864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7df7c6f834dd58c1afbd8a64abe410fc1e80ec544708fa9a965f57ab86a1d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:15:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:15:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:15:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 08:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:15:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:15:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:15:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf7daeb76c3bb0b9919f840ee1313d7bf03e238f25ccfa50685ba22c0a0948`  
		Last Modified: Fri, 11 Dec 2020 08:16:06 GMT  
		Size: 7.9 MB (7928844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b6373b354ba393226a1d7e15beb5d3919235aebaad2e462b77a90718b558e`  
		Last Modified: Fri, 11 Dec 2020 08:16:04 GMT  
		Size: 1.3 MB (1327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1a1637bd896f4e26717e8304024ce908354fa2dc98efa5cc9f259041d9e42`  
		Last Modified: Fri, 11 Dec 2020 08:16:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d4ebeec4a896b43b05053e5f61d4d78aebf77717043d77fcae5f8b903ad10631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118414315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3467a549ea0fdd27eab9873a3dc66116f589f7fb59ddfcfce4d3e0754b62f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:55 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 16:39:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433be6df8d40c95a43238d4562dc038798dbafe8378275ac6f7892c47c2556d`  
		Last Modified: Fri, 11 Dec 2020 16:40:50 GMT  
		Size: 8.4 MB (8352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bae692d5a8f8b212bd467f34afe61584d54eb7761d05104582b79fa0590a52f`  
		Last Modified: Fri, 11 Dec 2020 16:40:48 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64532095c920265ad0fe12449c16c4c91e2f65d579d594917175d9b0f79e71bd`  
		Last Modified: Fri, 11 Dec 2020 16:40:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ff83752ca71e5b02a7d7b34f958ec282c6c7d2118f8cfd096675df206daf47ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:2.2.1-builder-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:243fdb842eb0ae5c699a0b2c6b21e073188b55d46b5f1676019f0f095ffca10f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565628646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba058fb2a4eb196ac68f44e313a930f00c616e461f23e6bfa1edf451b3b3bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:55:28 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:55:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:55:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:55:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206310242577d11bd5feb3aa11b5f7d090a6edc146c4b229e6a4975cf73c1286`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903040d044b4614ed82d2ea5c95b10d236be0d4e4663b746f0c926fec5da92f`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0805737182f599ffeb040b6aa7f9338886390514b97d8ad6a9d020416344b`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad7c66c28d14e3a2438621bd6ce3eb16838bc04cec4e38be4022719b6b2ec9`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123020c4e3f3f7ca21810e8fbd2ce260e1962aa76fe2ddef3044a6e7614a10f8`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.8 MB (1761375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85eee7c96161123b7862f2e6ef2594e84968b082fd7f819a0c26ed08d476a30`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6c06e2c038375f9863689a4c7a743a66faffe9bdcd1aee2308b542d7d5c49f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.2.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:b75948041fc580c0d1edd8aa722a8277bb301ba41d8b590a4f17c66c9fe4ab40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964606778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a2250a1f590dde32f7e679b96a04ed050c4655a60ae952af73b0c26d598c80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:59 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:56:00 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:56:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:57:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:57:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4e04e74a87b1fb4ec35b081bb61d4e85f9f0b3a80c88d8a44a20efc94584e`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342b3373ee29de0d987f0b40171c41395e9b00269cab4de6dbf2a90503cef74`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973292c9e2947dc0e10764597f6f9f50d9e521151f3f1ffce12110bd59d7ac9`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeda6d1d0446d45cf769ad800da810928a915a53f0f15741d1f2d5e330bfbd`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03028d69a4efd9fca773e4c828323c76cc768d9f5842bff350846206e20642c6`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 11.5 MB (11462074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5c946ea76708b5d1b6c1393f0d926d12c16e5eac35699436370388d806e55`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore`

```console
$ docker pull caddy@sha256:94222b11fa710228c495d0963ae695e54d8e8e5ef631517a00f7e2557465e82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.2.1-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6f9fa402f617af6a08a77a3d6821621bb5bb0f3b99080d2d9b8d990104a3fb48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:358936d5db6ea416ac9bd28395c579cf0f12fe0f53065eff3dd7a6e1ec101ecb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:a4d99ca9d9c9c0b2c8bd2ffe356ed4ca5e0ebe5141a09af64b5ff72a71f7d72f
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
$ docker pull caddy@sha256:5c14834055e3ec0800789a46db92258f78556ef9971457022234e3487c2ae207
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4daabe9339412068d7bcc4c9b0ac275c67c82d8c819e4b37a387b50fa8e9a61b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:28:21 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:28 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4428f13c7edb68201eb53fc2a833e3e1831b1bfc66d8ca591d7d7981e8dcdb57`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b931870cc5c313c5b12bd911762577180c41684025e803ac19870628f24474`  
		Last Modified: Fri, 11 Dec 2020 02:29:11 GMT  
		Size: 11.5 MB (11532507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010bdd923cf20d340b6e9f06cac8c3f1e1984172c4f4d095cd9b443b03ad818`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ee965d543057e5cb4af597d364066251a9852583059cd38488243306b724a778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7753d72769487802d1fee3d3f07ee3ce735418d63d93259ad8125a3ae2de1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:10:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:10:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:10:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:10:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:10:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:10:21 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:10:21 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:10:22 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:10:23 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:10:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:10:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:10:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:10:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:10:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:10:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:10:31 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:10:32 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:10:33 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:10:35 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:10:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7ab50db8ca6e467811f1281518708c79ffb3eba857ede634fe075aa109cf4`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c5497e98ba2efc52fb51339d08617c1ffc210163f8774632f307c81683deb`  
		Last Modified: Fri, 11 Dec 2020 03:11:27 GMT  
		Size: 10.9 MB (10876275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140a3a819ce00971b2089202730b7c285ca9a6ab1f5832820b20a043fd51fcc9`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2d82fb7e660d56846fa3c33deb953bfc6c464bfb8fba608c237b4a5e0eee33c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e57be32d04a04308b9f9c3fcbac701e798783ecbe10f243a411262f5a05cb0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:07:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:07:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:07:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:07:14 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:07:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:07:16 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:07:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:07:18 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:07:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:07:24 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:07:25 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:07:26 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:07:27 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:07:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2348443ed0fb4b09e2d5b6d636d90e4bbf2024e934143fadfcc35bbc65a709a1`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8462380e6876aca9643bcf369ffc7b958a08c3fd3fc56a861ca651a1fcaf9c`  
		Last Modified: Fri, 11 Dec 2020 03:08:19 GMT  
		Size: 10.9 MB (10854381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7839ddc84cd5ea73da141c2726d80c7493a37772c128eb7f60b1621784acf0`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8a8a108facaeb348bc873b80764a0e142fa06279dce55fc16f6d68017de99f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b781915644b6cb14f7dbcb44242df9845f6f989c96c3b75da745a4c11d116ca0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:33:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:33:42 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:33:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:33:52 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:33:53 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:34:00 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:34:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:34:03 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:34:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:34:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:34:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:34:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:34:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:34:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:34:19 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:34:21 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:34:23 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:34:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a6157741b4baecc6781d3a2227bd753df1a152366cfba7d5f83731611b38f3`  
		Last Modified: Fri, 11 Dec 2020 03:35:17 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f6d968230fb7b05d7bb6b35f8eab026c6e68c93458a9c40095b9bccb7eb23d`  
		Last Modified: Fri, 11 Dec 2020 03:35:20 GMT  
		Size: 10.5 MB (10527460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665b752f90ad5d8f5f8c6840c5cc58eb1b542c21773b827303c156732f73321`  
		Last Modified: Fri, 11 Dec 2020 03:35:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b5c5d0c317892db3c940899c940405ad1283f0857b3cb1c454abce45a325b8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf8c3b1e29b5c01bce118fbc104af2924a4b50324db40dedeb78ba2d9df4c33`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 06:44:22 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 06:44:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:44:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:44:48 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:44:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:44:54 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:44:57 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:45:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 06:45:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:45:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:45:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:45:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:45:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:45:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:45:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:45:35 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:45:39 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:45:45 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:45:49 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:45:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f10029b2ed0c8a52065e9b56b5b27d4f7a83fcba0392c7021532236b70a0f`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd4c79b504a226097858b4a8bc37dbed1031f3a3205cf552a5ebceb132f791`  
		Last Modified: Fri, 11 Dec 2020 06:46:51 GMT  
		Size: 10.2 MB (10180214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2cc34795b6c9d9081692bd53a1f7b77ae6a7c9e9e661f863cc493d6973a26`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:90b5dcd8d713f82a46c2039baee451f911f8d25f27431e6b44655f8b2803c557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f49a1c397b4a9cdc0f9a6cd1eb6aea12154952a3d4ead09ddd6c9595bb4361`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:43:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:43:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:50 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752f95e37b35ec8cf81bd3caab7ba2ea836620747fa2d720c5b64709254ddae`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f574024c894c439da18a68fa9e20ef03be94dd77a2b1934242463f93d518b0`  
		Last Modified: Fri, 11 Dec 2020 02:44:34 GMT  
		Size: 11.2 MB (11202556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26947b55683beda16dec6f01fc3ef037d91c61349dae0527952bafce3c03d5c0`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:9f749efb38b7060cb073368176598d2bea4c67e8f9f050ead321ff78cae40310
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:b096584711e39f807c8aeb0924293459032118282197f3a5cea41c42622651d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119507588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9648450acd39780f89804ab3007ad951549a488ac54ada25330077688ad01f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:20:38 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:20:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:20:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:20:40 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:24:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:24:02 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:24:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:24:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:24:04 GMT
WORKDIR /go
# Fri, 11 Dec 2020 22:11:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 22:11:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 22:11:47 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 22:11:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 22:11:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 22:11:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 22:11:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bcff5d981b47d576e4ee185cfc784f975e2fb191f463b5c579fc5cf003f88d`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 280.8 KB (280796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a343aaa7d2b207b798539017dfc6c3cb3f6043240b793f313c4439535b4855`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2128e2ad96160c85ca6f26a5c5ca34b05d1358c90ab539d38e0365affc9a2e`  
		Last Modified: Fri, 11 Dec 2020 05:28:00 GMT  
		Size: 106.7 MB (106711940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3766394496033d48e3f79c602e0a29249ebcd72c6c50b4c4749717acc8734b5`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac1c34c07ea45a1dd2a140ef4773c39f4fa2ec603422da061121ff393ce0e07`  
		Last Modified: Fri, 11 Dec 2020 22:12:24 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ff964ba9844f52702d26570857e396f4294a36b58cce1484fb1f20bca16d3`  
		Last Modified: Fri, 11 Dec 2020 22:12:24 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62786d114c16e2a05f5c9717ebd63270f32c431d50ec1eb429e127688252b4c`  
		Last Modified: Fri, 11 Dec 2020 22:12:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:5dd4797c97ea381ace1e1eea532fd5f29423ac06b12c619cafe000d64509feb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114700864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7df7c6f834dd58c1afbd8a64abe410fc1e80ec544708fa9a965f57ab86a1d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:15:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:15:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:15:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 08:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:15:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:15:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:15:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf7daeb76c3bb0b9919f840ee1313d7bf03e238f25ccfa50685ba22c0a0948`  
		Last Modified: Fri, 11 Dec 2020 08:16:06 GMT  
		Size: 7.9 MB (7928844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b6373b354ba393226a1d7e15beb5d3919235aebaad2e462b77a90718b558e`  
		Last Modified: Fri, 11 Dec 2020 08:16:04 GMT  
		Size: 1.3 MB (1327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1a1637bd896f4e26717e8304024ce908354fa2dc98efa5cc9f259041d9e42`  
		Last Modified: Fri, 11 Dec 2020 08:16:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:d4ebeec4a896b43b05053e5f61d4d78aebf77717043d77fcae5f8b903ad10631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118414315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3467a549ea0fdd27eab9873a3dc66116f589f7fb59ddfcfce4d3e0754b62f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:55 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 16:39:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433be6df8d40c95a43238d4562dc038798dbafe8378275ac6f7892c47c2556d`  
		Last Modified: Fri, 11 Dec 2020 16:40:50 GMT  
		Size: 8.4 MB (8352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bae692d5a8f8b212bd467f34afe61584d54eb7761d05104582b79fa0590a52f`  
		Last Modified: Fri, 11 Dec 2020 16:40:48 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64532095c920265ad0fe12449c16c4c91e2f65d579d594917175d9b0f79e71bd`  
		Last Modified: Fri, 11 Dec 2020 16:40:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:243fdb842eb0ae5c699a0b2c6b21e073188b55d46b5f1676019f0f095ffca10f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565628646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba058fb2a4eb196ac68f44e313a930f00c616e461f23e6bfa1edf451b3b3bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:55:28 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:55:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:55:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:55:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206310242577d11bd5feb3aa11b5f7d090a6edc146c4b229e6a4975cf73c1286`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903040d044b4614ed82d2ea5c95b10d236be0d4e4663b746f0c926fec5da92f`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0805737182f599ffeb040b6aa7f9338886390514b97d8ad6a9d020416344b`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad7c66c28d14e3a2438621bd6ce3eb16838bc04cec4e38be4022719b6b2ec9`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123020c4e3f3f7ca21810e8fbd2ce260e1962aa76fe2ddef3044a6e7614a10f8`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.8 MB (1761375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85eee7c96161123b7862f2e6ef2594e84968b082fd7f819a0c26ed08d476a30`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:b75948041fc580c0d1edd8aa722a8277bb301ba41d8b590a4f17c66c9fe4ab40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964606778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a2250a1f590dde32f7e679b96a04ed050c4655a60ae952af73b0c26d598c80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:59 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:56:00 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:56:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:57:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:57:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4e04e74a87b1fb4ec35b081bb61d4e85f9f0b3a80c88d8a44a20efc94584e`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342b3373ee29de0d987f0b40171c41395e9b00269cab4de6dbf2a90503cef74`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973292c9e2947dc0e10764597f6f9f50d9e521151f3f1ffce12110bd59d7ac9`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeda6d1d0446d45cf769ad800da810928a915a53f0f15741d1f2d5e330bfbd`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03028d69a4efd9fca773e4c828323c76cc768d9f5842bff350846206e20642c6`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 11.5 MB (11462074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5c946ea76708b5d1b6c1393f0d926d12c16e5eac35699436370388d806e55`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:1f215f875df2c1ebf5a3353c9d1b8f4c9d5c00702f9df037af1955fc86bf422b
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
$ docker pull caddy@sha256:b096584711e39f807c8aeb0924293459032118282197f3a5cea41c42622651d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119507588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9648450acd39780f89804ab3007ad951549a488ac54ada25330077688ad01f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:20:38 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:20:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:20:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:20:40 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:24:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:24:02 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:24:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:24:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:24:04 GMT
WORKDIR /go
# Fri, 11 Dec 2020 22:11:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 22:11:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 22:11:47 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 22:11:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 22:11:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 22:11:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 22:11:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bcff5d981b47d576e4ee185cfc784f975e2fb191f463b5c579fc5cf003f88d`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 280.8 KB (280796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a343aaa7d2b207b798539017dfc6c3cb3f6043240b793f313c4439535b4855`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2128e2ad96160c85ca6f26a5c5ca34b05d1358c90ab539d38e0365affc9a2e`  
		Last Modified: Fri, 11 Dec 2020 05:28:00 GMT  
		Size: 106.7 MB (106711940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3766394496033d48e3f79c602e0a29249ebcd72c6c50b4c4749717acc8734b5`  
		Last Modified: Fri, 11 Dec 2020 05:27:35 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac1c34c07ea45a1dd2a140ef4773c39f4fa2ec603422da061121ff393ce0e07`  
		Last Modified: Fri, 11 Dec 2020 22:12:24 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ff964ba9844f52702d26570857e396f4294a36b58cce1484fb1f20bca16d3`  
		Last Modified: Fri, 11 Dec 2020 22:12:24 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62786d114c16e2a05f5c9717ebd63270f32c431d50ec1eb429e127688252b4c`  
		Last Modified: Fri, 11 Dec 2020 22:12:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:5dd4797c97ea381ace1e1eea532fd5f29423ac06b12c619cafe000d64509feb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114700864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7df7c6f834dd58c1afbd8a64abe410fc1e80ec544708fa9a965f57ab86a1d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:15:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:15:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:15:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 08:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:15:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:15:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:15:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf7daeb76c3bb0b9919f840ee1313d7bf03e238f25ccfa50685ba22c0a0948`  
		Last Modified: Fri, 11 Dec 2020 08:16:06 GMT  
		Size: 7.9 MB (7928844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b6373b354ba393226a1d7e15beb5d3919235aebaad2e462b77a90718b558e`  
		Last Modified: Fri, 11 Dec 2020 08:16:04 GMT  
		Size: 1.3 MB (1327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1a1637bd896f4e26717e8304024ce908354fa2dc98efa5cc9f259041d9e42`  
		Last Modified: Fri, 11 Dec 2020 08:16:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d4ebeec4a896b43b05053e5f61d4d78aebf77717043d77fcae5f8b903ad10631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118414315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3467a549ea0fdd27eab9873a3dc66116f589f7fb59ddfcfce4d3e0754b62f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:55 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 16:39:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433be6df8d40c95a43238d4562dc038798dbafe8378275ac6f7892c47c2556d`  
		Last Modified: Fri, 11 Dec 2020 16:40:50 GMT  
		Size: 8.4 MB (8352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bae692d5a8f8b212bd467f34afe61584d54eb7761d05104582b79fa0590a52f`  
		Last Modified: Fri, 11 Dec 2020 16:40:48 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64532095c920265ad0fe12449c16c4c91e2f65d579d594917175d9b0f79e71bd`  
		Last Modified: Fri, 11 Dec 2020 16:40:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ff83752ca71e5b02a7d7b34f958ec282c6c7d2118f8cfd096675df206daf47ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:243fdb842eb0ae5c699a0b2c6b21e073188b55d46b5f1676019f0f095ffca10f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565628646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba058fb2a4eb196ac68f44e313a930f00c616e461f23e6bfa1edf451b3b3bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:55:28 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:55:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:55:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:55:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206310242577d11bd5feb3aa11b5f7d090a6edc146c4b229e6a4975cf73c1286`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903040d044b4614ed82d2ea5c95b10d236be0d4e4663b746f0c926fec5da92f`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0805737182f599ffeb040b6aa7f9338886390514b97d8ad6a9d020416344b`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad7c66c28d14e3a2438621bd6ce3eb16838bc04cec4e38be4022719b6b2ec9`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123020c4e3f3f7ca21810e8fbd2ce260e1962aa76fe2ddef3044a6e7614a10f8`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.8 MB (1761375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85eee7c96161123b7862f2e6ef2594e84968b082fd7f819a0c26ed08d476a30`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6c06e2c038375f9863689a4c7a743a66faffe9bdcd1aee2308b542d7d5c49f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:b75948041fc580c0d1edd8aa722a8277bb301ba41d8b590a4f17c66c9fe4ab40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964606778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a2250a1f590dde32f7e679b96a04ed050c4655a60ae952af73b0c26d598c80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:59 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:56:00 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:56:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:57:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:57:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4e04e74a87b1fb4ec35b081bb61d4e85f9f0b3a80c88d8a44a20efc94584e`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342b3373ee29de0d987f0b40171c41395e9b00269cab4de6dbf2a90503cef74`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973292c9e2947dc0e10764597f6f9f50d9e521151f3f1ffce12110bd59d7ac9`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeda6d1d0446d45cf769ad800da810928a915a53f0f15741d1f2d5e330bfbd`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03028d69a4efd9fca773e4c828323c76cc768d9f5842bff350846206e20642c6`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 11.5 MB (11462074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5c946ea76708b5d1b6c1393f0d926d12c16e5eac35699436370388d806e55`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:94222b11fa710228c495d0963ae695e54d8e8e5ef631517a00f7e2557465e82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6f9fa402f617af6a08a77a3d6821621bb5bb0f3b99080d2d9b8d990104a3fb48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:358936d5db6ea416ac9bd28395c579cf0f12fe0f53065eff3dd7a6e1ec101ecb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:a4d99ca9d9c9c0b2c8bd2ffe356ed4ca5e0ebe5141a09af64b5ff72a71f7d72f
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
$ docker pull caddy@sha256:5c14834055e3ec0800789a46db92258f78556ef9971457022234e3487c2ae207
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4daabe9339412068d7bcc4c9b0ac275c67c82d8c819e4b37a387b50fa8e9a61b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:28:21 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:28 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4428f13c7edb68201eb53fc2a833e3e1831b1bfc66d8ca591d7d7981e8dcdb57`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b931870cc5c313c5b12bd911762577180c41684025e803ac19870628f24474`  
		Last Modified: Fri, 11 Dec 2020 02:29:11 GMT  
		Size: 11.5 MB (11532507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010bdd923cf20d340b6e9f06cac8c3f1e1984172c4f4d095cd9b443b03ad818`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ee965d543057e5cb4af597d364066251a9852583059cd38488243306b724a778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7753d72769487802d1fee3d3f07ee3ce735418d63d93259ad8125a3ae2de1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:10:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:10:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:10:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:10:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:10:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:10:21 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:10:21 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:10:22 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:10:23 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:10:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:10:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:10:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:10:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:10:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:10:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:10:31 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:10:32 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:10:33 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:10:35 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:10:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7ab50db8ca6e467811f1281518708c79ffb3eba857ede634fe075aa109cf4`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c5497e98ba2efc52fb51339d08617c1ffc210163f8774632f307c81683deb`  
		Last Modified: Fri, 11 Dec 2020 03:11:27 GMT  
		Size: 10.9 MB (10876275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140a3a819ce00971b2089202730b7c285ca9a6ab1f5832820b20a043fd51fcc9`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2d82fb7e660d56846fa3c33deb953bfc6c464bfb8fba608c237b4a5e0eee33c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e57be32d04a04308b9f9c3fcbac701e798783ecbe10f243a411262f5a05cb0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:07:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:07:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:07:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:07:14 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:07:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:07:16 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:07:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:07:18 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:07:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:07:24 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:07:25 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:07:26 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:07:27 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:07:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2348443ed0fb4b09e2d5b6d636d90e4bbf2024e934143fadfcc35bbc65a709a1`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8462380e6876aca9643bcf369ffc7b958a08c3fd3fc56a861ca651a1fcaf9c`  
		Last Modified: Fri, 11 Dec 2020 03:08:19 GMT  
		Size: 10.9 MB (10854381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7839ddc84cd5ea73da141c2726d80c7493a37772c128eb7f60b1621784acf0`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8a8a108facaeb348bc873b80764a0e142fa06279dce55fc16f6d68017de99f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b781915644b6cb14f7dbcb44242df9845f6f989c96c3b75da745a4c11d116ca0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:33:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:33:42 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:33:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:33:52 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:33:53 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:34:00 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:34:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:34:03 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:34:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:34:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:34:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:34:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:34:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:34:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:34:19 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:34:21 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:34:23 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:34:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a6157741b4baecc6781d3a2227bd753df1a152366cfba7d5f83731611b38f3`  
		Last Modified: Fri, 11 Dec 2020 03:35:17 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f6d968230fb7b05d7bb6b35f8eab026c6e68c93458a9c40095b9bccb7eb23d`  
		Last Modified: Fri, 11 Dec 2020 03:35:20 GMT  
		Size: 10.5 MB (10527460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665b752f90ad5d8f5f8c6840c5cc58eb1b542c21773b827303c156732f73321`  
		Last Modified: Fri, 11 Dec 2020 03:35:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b5c5d0c317892db3c940899c940405ad1283f0857b3cb1c454abce45a325b8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf8c3b1e29b5c01bce118fbc104af2924a4b50324db40dedeb78ba2d9df4c33`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 06:44:22 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 06:44:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:44:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:44:48 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:44:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:44:54 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:44:57 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:45:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 06:45:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:45:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:45:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:45:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:45:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:45:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:45:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:45:35 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:45:39 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:45:45 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:45:49 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:45:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f10029b2ed0c8a52065e9b56b5b27d4f7a83fcba0392c7021532236b70a0f`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd4c79b504a226097858b4a8bc37dbed1031f3a3205cf552a5ebceb132f791`  
		Last Modified: Fri, 11 Dec 2020 06:46:51 GMT  
		Size: 10.2 MB (10180214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2cc34795b6c9d9081692bd53a1f7b77ae6a7c9e9e661f863cc493d6973a26`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:90b5dcd8d713f82a46c2039baee451f911f8d25f27431e6b44655f8b2803c557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f49a1c397b4a9cdc0f9a6cd1eb6aea12154952a3d4ead09ddd6c9595bb4361`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:43:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:43:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:50 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752f95e37b35ec8cf81bd3caab7ba2ea836620747fa2d720c5b64709254ddae`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f574024c894c439da18a68fa9e20ef03be94dd77a2b1934242463f93d518b0`  
		Last Modified: Fri, 11 Dec 2020 02:44:34 GMT  
		Size: 11.2 MB (11202556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26947b55683beda16dec6f01fc3ef037d91c61349dae0527952bafce3c03d5c0`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:f6c2dae67ff30eb30043f191a9666b390ade3f947c76c2d4f1e917ccd3767f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:5dd4797c97ea381ace1e1eea532fd5f29423ac06b12c619cafe000d64509feb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114700864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7df7c6f834dd58c1afbd8a64abe410fc1e80ec544708fa9a965f57ab86a1d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:15:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:15:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:15:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 08:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:15:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:15:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:15:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf7daeb76c3bb0b9919f840ee1313d7bf03e238f25ccfa50685ba22c0a0948`  
		Last Modified: Fri, 11 Dec 2020 08:16:06 GMT  
		Size: 7.9 MB (7928844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b6373b354ba393226a1d7e15beb5d3919235aebaad2e462b77a90718b558e`  
		Last Modified: Fri, 11 Dec 2020 08:16:04 GMT  
		Size: 1.3 MB (1327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1a1637bd896f4e26717e8304024ce908354fa2dc98efa5cc9f259041d9e42`  
		Last Modified: Fri, 11 Dec 2020 08:16:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:d4ebeec4a896b43b05053e5f61d4d78aebf77717043d77fcae5f8b903ad10631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118414315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3467a549ea0fdd27eab9873a3dc66116f589f7fb59ddfcfce4d3e0754b62f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:55 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 16:39:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433be6df8d40c95a43238d4562dc038798dbafe8378275ac6f7892c47c2556d`  
		Last Modified: Fri, 11 Dec 2020 16:40:50 GMT  
		Size: 8.4 MB (8352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bae692d5a8f8b212bd467f34afe61584d54eb7761d05104582b79fa0590a52f`  
		Last Modified: Fri, 11 Dec 2020 16:40:48 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64532095c920265ad0fe12449c16c4c91e2f65d579d594917175d9b0f79e71bd`  
		Last Modified: Fri, 11 Dec 2020 16:40:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:243fdb842eb0ae5c699a0b2c6b21e073188b55d46b5f1676019f0f095ffca10f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565628646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba058fb2a4eb196ac68f44e313a930f00c616e461f23e6bfa1edf451b3b3bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:55:28 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:55:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:55:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:55:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206310242577d11bd5feb3aa11b5f7d090a6edc146c4b229e6a4975cf73c1286`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903040d044b4614ed82d2ea5c95b10d236be0d4e4663b746f0c926fec5da92f`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0805737182f599ffeb040b6aa7f9338886390514b97d8ad6a9d020416344b`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad7c66c28d14e3a2438621bd6ce3eb16838bc04cec4e38be4022719b6b2ec9`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123020c4e3f3f7ca21810e8fbd2ce260e1962aa76fe2ddef3044a6e7614a10f8`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.8 MB (1761375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85eee7c96161123b7862f2e6ef2594e84968b082fd7f819a0c26ed08d476a30`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:b75948041fc580c0d1edd8aa722a8277bb301ba41d8b590a4f17c66c9fe4ab40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964606778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a2250a1f590dde32f7e679b96a04ed050c4655a60ae952af73b0c26d598c80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:59 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:56:00 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:56:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:57:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:57:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4e04e74a87b1fb4ec35b081bb61d4e85f9f0b3a80c88d8a44a20efc94584e`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342b3373ee29de0d987f0b40171c41395e9b00269cab4de6dbf2a90503cef74`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973292c9e2947dc0e10764597f6f9f50d9e521151f3f1ffce12110bd59d7ac9`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeda6d1d0446d45cf769ad800da810928a915a53f0f15741d1f2d5e330bfbd`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03028d69a4efd9fca773e4c828323c76cc768d9f5842bff350846206e20642c6`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 11.5 MB (11462074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5c946ea76708b5d1b6c1393f0d926d12c16e5eac35699436370388d806e55`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:a0597f0650078a269e9d2c9b1e69bf3a13e695884ee2a9342df0d860d6b5e3a9
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
$ docker pull caddy@sha256:d7b066e0ae6a58162afa38de124bde6cafbcf0a7f4d056489ce88cc394471bed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e2ef96ee9bf6c12304aac59194314ca7a1e076d5904b34eac04d61337d964`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:34:56 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:34:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:34:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:21:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:24:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:24:09 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:24:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:24:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:24:10 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:49:11 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:49:12 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:49:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:49:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef7d3d256c8367c41c431143c63d083a25dd62ec9ee9d9773dd9e6c7b70ec9e`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 280.8 KB (280812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9db76c5a1d06710ed4f3073476b2d883ff8e911f8e47c558bc4a8d1d8663fa`  
		Last Modified: Thu, 22 Oct 2020 03:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b5e3429cf30be490cdf3c5018e8693e0e1d319ea295c9b0c37dedaa7a1cafb`  
		Last Modified: Fri, 04 Dec 2020 00:31:08 GMT  
		Size: 107.1 MB (107085919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6a0961518234df34a1cf391ec7269a68b99fc112f60e8a7270db07eb3974`  
		Last Modified: Fri, 04 Dec 2020 00:30:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe1a6296183cbfcabe79353a47f9336d847b7ea66b4fb61ae86fc689de5d77`  
		Last Modified: Fri, 04 Dec 2020 00:49:47 GMT  
		Size: 8.3 MB (8309940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da5ba704ae92109544c4683fde8e8be5eea27b6110540c808341c3b43145c6`  
		Last Modified: Fri, 04 Dec 2020 00:49:45 GMT  
		Size: 1.4 MB (1407200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572698d0ecf1dba5c0b8c6a996637e0de1f7e30e2901dae6927647fc8e0d63e7`  
		Last Modified: Fri, 04 Dec 2020 00:49:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:5dd4797c97ea381ace1e1eea532fd5f29423ac06b12c619cafe000d64509feb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114700864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7df7c6f834dd58c1afbd8a64abe410fc1e80ec544708fa9a965f57ab86a1d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:01:51 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 05:01:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:01:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:01:55 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 05:04:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 05:04:41 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 05:04:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 05:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 05:04:46 GMT
WORKDIR /go
# Fri, 11 Dec 2020 08:15:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 08:15:06 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 08:15:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 08:15:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 08:15:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 08:15:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 08:15:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c54fb8a883364d44abe49903dc93546608e4be42299daf298ec0bf7d6774e`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 281.0 KB (280988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2330f20a2b2cb3bbef000f0a21e2e96505df7a101a96d9a3d64d6760512fb9`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d8c53a4ee3be371b79034d561557cf2baa089fea4ef82f543b6a5dbe1cad8`  
		Last Modified: Fri, 11 Dec 2020 05:09:10 GMT  
		Size: 102.6 MB (102560978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e48cebf375fe9c16f6944ab4921d5803644884d872978e5d553df5188bda1ad`  
		Last Modified: Fri, 11 Dec 2020 05:08:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaf7daeb76c3bb0b9919f840ee1313d7bf03e238f25ccfa50685ba22c0a0948`  
		Last Modified: Fri, 11 Dec 2020 08:16:06 GMT  
		Size: 7.9 MB (7928844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b6373b354ba393226a1d7e15beb5d3919235aebaad2e462b77a90718b558e`  
		Last Modified: Fri, 11 Dec 2020 08:16:04 GMT  
		Size: 1.3 MB (1327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1a1637bd896f4e26717e8304024ce908354fa2dc98efa5cc9f259041d9e42`  
		Last Modified: Fri, 11 Dec 2020 08:16:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd9531e4414b412e4a1bdb2fbe16e0c83e38c8d058aaa93a6a40245cfd5c8f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.9 MB (113880893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3158c399bfa2628c5054f9d4e14c2dd225c2b4a45b8130026e462667ba683ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:21:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 03:23:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:23:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:03:17 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:05:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 00:05:41 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 00:05:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 00:05:44 GMT
WORKDIR /go
# Fri, 04 Dec 2020 00:33:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 00:33:33 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 00:33:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 00:33:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 00:33:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 00:33:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b753cfc04fdce9640aac1e7a4b3e7ce15fa60b8e357376e42f294f463a6e890`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 280.1 KB (280084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90c422e5e4668cb4140aadb622d734faa93c81cc1e283da9b08bbbc65c45c5`  
		Last Modified: Thu, 22 Oct 2020 05:59:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c37b023a65a717d26fdb8c72bba66adc8625ca96fab4d08e70954da6b10139`  
		Last Modified: Fri, 04 Dec 2020 00:14:22 GMT  
		Size: 102.7 MB (102723691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f091034d1629ecd6c35f9bbcb2754721bbfa4e5183794ff2b6ecc75b7b2e0e`  
		Last Modified: Fri, 04 Dec 2020 00:13:47 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809b32049841fc890dd29c935db10e86e95c4005906b5eddc3fa42f131cdb5`  
		Last Modified: Fri, 04 Dec 2020 00:34:08 GMT  
		Size: 7.1 MB (7144891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ba8d461e1618211000580b6f229d2fd9775115c3c4049fb7be235094e0625`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 1.3 MB (1325838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af262af67e01cb4ef945fd8c992860308e9509dc4810d2cab9ed6955b52a700`  
		Last Modified: Fri, 04 Dec 2020 00:34:07 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3bd8e226aa9f4fef563f2a76b0c165434ab3145a2b629512dcab6495c677202c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115210346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5e537fc1b6fe653ff07e33f1a30ba036846e07eb585a5a75815eeabb89e21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:08:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 04:09:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 04:09:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 00:59:20 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:01:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:01:23 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:01:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:01:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:01:29 GMT
WORKDIR /go
# Fri, 04 Dec 2020 01:28:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 01:28:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 01:28:28 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 01:28:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 01:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 01:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 01:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4357932f1b6fb010e1461cc5c673712fb832ac44ee627c691db0b64adf95d13`  
		Last Modified: Thu, 22 Oct 2020 04:28:32 GMT  
		Size: 281.2 KB (281230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c013af1878066e59b688e31fd962e7267430963de27c5257241e3c223aa1d6`  
		Last Modified: Thu, 22 Oct 2020 04:28:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37128a32d7b17416d88331ec94958c63f643120f6e40870110ef00f387be80e5`  
		Last Modified: Fri, 04 Dec 2020 01:09:15 GMT  
		Size: 102.4 MB (102411796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0279cf9b51b6c7d1d4937560cb5536f262e9f4e9c5a1685489387c9753062e04`  
		Last Modified: Fri, 04 Dec 2020 01:08:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed38fb55682cdaae259822fc0a1e349a7992f9f99404e4bdc58b4bee6e75d059`  
		Last Modified: Fri, 04 Dec 2020 01:29:03 GMT  
		Size: 8.5 MB (8499869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fdec9db4728520c427e5ae86d67521591251e09a667e19f8e6d0419c50d24`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 1.3 MB (1310181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96eec8ba730f3d05a0aac92b2d5d603ab21395ee6bd7cd3a0dcb0d80a1e4c96`  
		Last Modified: Fri, 04 Dec 2020 01:29:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8ad160201c4f5ecf7844ef8865006660c67a29f3ded38b197e4d1ceac08966ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114386918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c06890463e50025481be858d0e654711df6c38fe2c7236f9c20dabbd7038590`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:27:26 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 22 Oct 2020 13:27:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:56:29 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 01:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 04 Dec 2020 01:58:26 GMT
ENV GOPATH=/go
# Fri, 04 Dec 2020 01:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Dec 2020 01:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 04 Dec 2020 01:58:38 GMT
WORKDIR /go
# Fri, 04 Dec 2020 03:13:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 04 Dec 2020 03:13:32 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 04 Dec 2020 03:13:36 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 04 Dec 2020 03:13:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 04 Dec 2020 03:13:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 04 Dec 2020 03:13:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 04 Dec 2020 03:14:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9900411dc7c8c88618743573bf89478d726007403bd002d8b00d21b7fecd40a`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd106374e3baf7eb8e3d8f7ffd4c364a35e57dcb3a89f8a153327a4c3fa3f9`  
		Last Modified: Thu, 22 Oct 2020 13:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c21191f366f1d0001ca2ec647fe3454179351700e264f9025f3efe636d5a2`  
		Last Modified: Fri, 04 Dec 2020 02:07:13 GMT  
		Size: 101.1 MB (101092006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3c970f8c564da928ce32db5cc7981e5bc4819b99016458cf9f2ceda95aa31`  
		Last Modified: Fri, 04 Dec 2020 02:06:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6379430057b0313b2aa26fed01de99735afdc60ab9085d4a8660e5bbaa2b5595`  
		Last Modified: Fri, 04 Dec 2020 03:14:44 GMT  
		Size: 8.9 MB (8919986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71eeeb13c478d19d8ddd430419adba93210219538a556c2f13d6888de61b01d`  
		Last Modified: Fri, 04 Dec 2020 03:14:43 GMT  
		Size: 1.3 MB (1287788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b553b21761e1bd135a537841af7ef976560d1e74642f117e38ae3254ddf4eb9`  
		Last Modified: Fri, 04 Dec 2020 03:14:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d4ebeec4a896b43b05053e5f61d4d78aebf77717043d77fcae5f8b903ad10631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118414315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3467a549ea0fdd27eab9873a3dc66116f589f7fb59ddfcfce4d3e0754b62f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:30:08 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 11 Dec 2020 03:30:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:30:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:30:11 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 11 Dec 2020 03:31:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.6.src.tar.gz'; 	sha256='890bba73c5e2b19ffb1180e385ea225059eb008eb91b694875dd86ea48675817'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 11 Dec 2020 03:32:05 GMT
ENV GOPATH=/go
# Fri, 11 Dec 2020 03:32:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 03:32:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 11 Dec 2020 03:32:06 GMT
WORKDIR /go
# Fri, 11 Dec 2020 16:39:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Dec 2020 16:39:55 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 11 Dec 2020 16:39:55 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 16:39:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Dec 2020 16:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Dec 2020 16:39:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Dec 2020 16:39:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b8373ee2322550f964161dcc28f9d31ea197b1b06dc0b208d66814fd56c7c`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 281.3 KB (281326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522c8c1c290acd48fd0576ff7b683af6c6810b571304e648801aa55ac3fc6d4`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7cf01ed0b10939a4565a6ba501d639022e8ae33a3601d3b154ea72128c3b3a`  
		Last Modified: Fri, 11 Dec 2020 03:35:23 GMT  
		Size: 105.8 MB (105825250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f330ba5036ee04e6172972318087882091d8b53b4936426ad450d1a0cfb514`  
		Last Modified: Fri, 11 Dec 2020 03:35:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433be6df8d40c95a43238d4562dc038798dbafe8378275ac6f7892c47c2556d`  
		Last Modified: Fri, 11 Dec 2020 16:40:50 GMT  
		Size: 8.4 MB (8352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bae692d5a8f8b212bd467f34afe61584d54eb7761d05104582b79fa0590a52f`  
		Last Modified: Fri, 11 Dec 2020 16:40:48 GMT  
		Size: 1.4 MB (1388752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64532095c920265ad0fe12449c16c4c91e2f65d579d594917175d9b0f79e71bd`  
		Last Modified: Fri, 11 Dec 2020 16:40:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ff83752ca71e5b02a7d7b34f958ec282c6c7d2118f8cfd096675df206daf47ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:243fdb842eb0ae5c699a0b2c6b21e073188b55d46b5f1676019f0f095ffca10f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565628646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ba058fb2a4eb196ac68f44e313a930f00c616e461f23e6bfa1edf451b3b3bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:30:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:30:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:30:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:31:35 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:31:57 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:31:58 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:34:28 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:34:29 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:27 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:55:28 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:55:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:55:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:55:53 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5287e7eabe2989764541d2d84c4676b838a30a6cf7582ae1634e551b3ef2f`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588b553e313f50806677aefb0ecff1b14bc3bf2af3502007ed9a8d56a8583fc5`  
		Last Modified: Wed, 09 Dec 2020 13:54:35 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbdf38d85835112bbd66c15c88fa10af5cc452590f50bed5c4eb114aef12e9`  
		Last Modified: Wed, 09 Dec 2020 13:54:34 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b50f011f5bd2ab0eaef775ba7b2f9a5fbb8d05f53f675cfb55480847fa80c3`  
		Last Modified: Wed, 09 Dec 2020 13:54:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9000bff3ee5b419217d7c208139db32357708f5e042073232d013021b9648`  
		Last Modified: Wed, 09 Dec 2020 13:54:39 GMT  
		Size: 34.3 MB (34329902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb549abdec7bb8d4debb3e8d9c2220fe8a39c707f3b55ca0041105f451407112`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766c92af76c17356f7a58754b35eef18ba39be13fac5c7122c2fdcf092668de`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 293.7 KB (293711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316565f55d31523fdfcb01911fc30d22ac533ba7caf3a6b1b1c82d4e5a1ba3ab`  
		Last Modified: Wed, 09 Dec 2020 13:54:25 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0d077fdd4cfce06b53ec657234fc70f93c76e7b88bbaa5e2688abfc5690507`  
		Last Modified: Wed, 09 Dec 2020 13:54:59 GMT  
		Size: 138.4 MB (138354476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0774b3459f90d7ddb0bf00cf559125df32dad069cd1666c5ed6303f427233fcb`  
		Last Modified: Wed, 09 Dec 2020 13:54:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206310242577d11bd5feb3aa11b5f7d090a6edc146c4b229e6a4975cf73c1286`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903040d044b4614ed82d2ea5c95b10d236be0d4e4663b746f0c926fec5da92f`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd0805737182f599ffeb040b6aa7f9338886390514b97d8ad6a9d020416344b`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad7c66c28d14e3a2438621bd6ce3eb16838bc04cec4e38be4022719b6b2ec9`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123020c4e3f3f7ca21810e8fbd2ce260e1962aa76fe2ddef3044a6e7614a10f8`  
		Last Modified: Wed, 09 Dec 2020 23:00:41 GMT  
		Size: 1.8 MB (1761375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85eee7c96161123b7862f2e6ef2594e84968b082fd7f819a0c26ed08d476a30`  
		Last Modified: Wed, 09 Dec 2020 23:00:37 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6c06e2c038375f9863689a4c7a743a66faffe9bdcd1aee2308b542d7d5c49f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:b75948041fc580c0d1edd8aa722a8277bb301ba41d8b590a4f17c66c9fe4ab40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964606778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a2250a1f590dde32f7e679b96a04ed050c4655a60ae952af73b0c26d598c80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Dec 2020 13:34:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Dec 2020 13:34:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Dec 2020 13:34:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Dec 2020 13:36:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:36:54 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Dec 2020 13:38:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Dec 2020 13:38:11 GMT
ENV GOLANG_VERSION=1.15.6
# Wed, 09 Dec 2020 13:41:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 13:41:43 GMT
WORKDIR C:\gopath
# Wed, 09 Dec 2020 22:55:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:55:59 GMT
ENV XCADDY_VERSION=v0.1.5
# Wed, 09 Dec 2020 22:56:00 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:56:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Dec 2020 22:57:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Dec 2020 22:57:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f374b7a81d8d1da3ea2e749c7510b6aa8464f5cf9cfd8635eee23c26c264186`  
		Last Modified: Wed, 09 Dec 2020 13:55:32 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c2e54f8832483cbe5f46ec46fd2932e9656680f47c5811d036e1f9c60f9b79`  
		Last Modified: Wed, 09 Dec 2020 13:55:30 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a357d7b727e3e4efaec8f4443236eb37c1fed68ca863b98d5b19ad17395225`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0785c68a2876dc32a5ff5aea8c9dbaddcea68864db06f5af609f3f65240a9`  
		Last Modified: Wed, 09 Dec 2020 13:55:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661765d49c7f605a23d3caa9a99455ce231aa2576dd72ff0b8eab7a5e2ec7ce6`  
		Last Modified: Wed, 09 Dec 2020 13:56:06 GMT  
		Size: 35.1 MB (35137422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d1f955bf7fa5325ae4ff054954789b3895bf8fab9ecc625537f8f673abd5`  
		Last Modified: Wed, 09 Dec 2020 13:55:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc55fb10a0bab3af9f2e63e7fcb33ba85af44f9e4877a85c0301a6114533edd`  
		Last Modified: Wed, 09 Dec 2020 13:55:26 GMT  
		Size: 5.5 MB (5497159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8203b1d27b0d111a6fbb09e09707cebb1991dc96c22cb61122d7b3a11c9ee`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa19bd5b077ef4c72c70c3a038e75d69dcf133835ba71839ee690433c01736f`  
		Last Modified: Wed, 09 Dec 2020 13:55:58 GMT  
		Size: 143.7 MB (143651420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5437279258059e7b08038e7ec5bd346c95f4bf73e1cb030bdd90ecd1128a7870`  
		Last Modified: Wed, 09 Dec 2020 13:55:25 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4e04e74a87b1fb4ec35b081bb61d4e85f9f0b3a80c88d8a44a20efc94584e`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342b3373ee29de0d987f0b40171c41395e9b00269cab4de6dbf2a90503cef74`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973292c9e2947dc0e10764597f6f9f50d9e521151f3f1ffce12110bd59d7ac9`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbeda6d1d0446d45cf769ad800da810928a915a53f0f15741d1f2d5e330bfbd`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03028d69a4efd9fca773e4c828323c76cc768d9f5842bff350846206e20642c6`  
		Last Modified: Wed, 09 Dec 2020 23:01:00 GMT  
		Size: 11.5 MB (11462074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5c946ea76708b5d1b6c1393f0d926d12c16e5eac35699436370388d806e55`  
		Last Modified: Wed, 09 Dec 2020 23:00:57 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:3bdc57eb2bf54c1df10c43fc566f1cc5269f6ae8a5b9a86e3b9fa98a614a66d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:5c14834055e3ec0800789a46db92258f78556ef9971457022234e3487c2ae207
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14635309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4daabe9339412068d7bcc4c9b0ac275c67c82d8c819e4b37a387b50fa8e9a61b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:28:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:28:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:28:21 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:28:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:28:25 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:28:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:28:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:28:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:28:27 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:28:28 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:28:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5605df8a1fb0ca66be628849d6c0ca12c0e472c9652ff8fd4ec82d45cac011`  
		Last Modified: Fri, 11 Dec 2020 02:29:00 GMT  
		Size: 299.9 KB (299945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4428f13c7edb68201eb53fc2a833e3e1831b1bfc66d8ca591d7d7981e8dcdb57`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b931870cc5c313c5b12bd911762577180c41684025e803ac19870628f24474`  
		Last Modified: Fri, 11 Dec 2020 02:29:11 GMT  
		Size: 11.5 MB (11532507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010bdd923cf20d340b6e9f06cac8c3f1e1984172c4f4d095cd9b443b03ad818`  
		Last Modified: Fri, 11 Dec 2020 02:29:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ee965d543057e5cb4af597d364066251a9852583059cd38488243306b724a778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13784367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7753d72769487802d1fee3d3f07ee3ce735418d63d93259ad8125a3ae2de1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:09:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:10:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:10:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:10:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:10:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:10:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:10:21 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:10:21 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:10:22 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:10:23 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:10:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:10:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:10:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:10:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:10:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:10:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:10:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:10:31 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:10:32 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:10:33 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:10:35 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:10:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b99de35a1926a351b1570538a0daebdec8818671a5888a2a050cd69e07311c`  
		Last Modified: Fri, 11 Dec 2020 03:11:13 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7ab50db8ca6e467811f1281518708c79ffb3eba857ede634fe075aa109cf4`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c5497e98ba2efc52fb51339d08617c1ffc210163f8774632f307c81683deb`  
		Last Modified: Fri, 11 Dec 2020 03:11:27 GMT  
		Size: 10.9 MB (10876275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140a3a819ce00971b2089202730b7c285ca9a6ab1f5832820b20a043fd51fcc9`  
		Last Modified: Fri, 11 Dec 2020 03:11:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2d82fb7e660d56846fa3c33deb953bfc6c464bfb8fba608c237b4a5e0eee33c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13565251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e57be32d04a04308b9f9c3fcbac701e798783ecbe10f243a411262f5a05cb0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:06:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:07:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:07:07 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:07:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:07:14 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:07:15 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:07:16 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:07:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:07:18 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:07:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:07:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:07:24 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:07:25 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:07:26 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:07:27 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:07:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dada83e01881dc169d8c4b56f8745a2ca2786a0632c41c34d585236d7a2472b9`  
		Last Modified: Fri, 11 Dec 2020 03:08:02 GMT  
		Size: 299.2 KB (299200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2348443ed0fb4b09e2d5b6d636d90e4bbf2024e934143fadfcc35bbc65a709a1`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8462380e6876aca9643bcf369ffc7b958a08c3fd3fc56a861ca651a1fcaf9c`  
		Last Modified: Fri, 11 Dec 2020 03:08:19 GMT  
		Size: 10.9 MB (10854381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7839ddc84cd5ea73da141c2726d80c7493a37772c128eb7f60b1621784acf0`  
		Last Modified: Fri, 11 Dec 2020 03:08:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8a8a108facaeb348bc873b80764a0e142fa06279dce55fc16f6d68017de99f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13540402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b781915644b6cb14f7dbcb44242df9845f6f989c96c3b75da745a4c11d116ca0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 03:33:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 03:33:42 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 03:33:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 03:33:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:33:52 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 03:33:53 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 03:34:00 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 03:34:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 03:34:03 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 03:34:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 03:34:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 03:34:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 03:34:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 03:34:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 03:34:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 03:34:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 03:34:19 GMT
EXPOSE 80
# Fri, 11 Dec 2020 03:34:21 GMT
EXPOSE 443
# Fri, 11 Dec 2020 03:34:23 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 03:34:25 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 03:34:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf15cb0f392d1155ad8b6d0f37777571d4db8c98af513a2d91f69db3fd0dd953`  
		Last Modified: Fri, 11 Dec 2020 03:35:02 GMT  
		Size: 300.3 KB (300339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a6157741b4baecc6781d3a2227bd753df1a152366cfba7d5f83731611b38f3`  
		Last Modified: Fri, 11 Dec 2020 03:35:17 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f6d968230fb7b05d7bb6b35f8eab026c6e68c93458a9c40095b9bccb7eb23d`  
		Last Modified: Fri, 11 Dec 2020 03:35:20 GMT  
		Size: 10.5 MB (10527460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665b752f90ad5d8f5f8c6840c5cc58eb1b542c21773b827303c156732f73321`  
		Last Modified: Fri, 11 Dec 2020 03:35:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:b5c5d0c317892db3c940899c940405ad1283f0857b3cb1c454abce45a325b8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf8c3b1e29b5c01bce118fbc104af2924a4b50324db40dedeb78ba2d9df4c33`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:42:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 06:44:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 06:44:22 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 06:44:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 06:44:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 06:44:48 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 06:44:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 06:44:54 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 06:44:57 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 06:45:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 06:45:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 06:45:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 06:45:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 06:45:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 06:45:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 06:45:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 06:45:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 06:45:35 GMT
EXPOSE 80
# Fri, 11 Dec 2020 06:45:39 GMT
EXPOSE 443
# Fri, 11 Dec 2020 06:45:45 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 06:45:49 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 06:45:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e202d5c41d5f69c28045becf50d14dda3860dd71696f675d3f66e48be375d4f`  
		Last Modified: Fri, 11 Dec 2020 06:46:35 GMT  
		Size: 302.3 KB (302333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f10029b2ed0c8a52065e9b56b5b27d4f7a83fcba0392c7021532236b70a0f`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd4c79b504a226097858b4a8bc37dbed1031f3a3205cf552a5ebceb132f791`  
		Last Modified: Fri, 11 Dec 2020 06:46:51 GMT  
		Size: 10.2 MB (10180214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2cc34795b6c9d9081692bd53a1f7b77ae6a7c9e9e661f863cc493d6973a26`  
		Last Modified: Fri, 11 Dec 2020 06:46:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:90b5dcd8d713f82a46c2039baee451f911f8d25f27431e6b44655f8b2803c557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14074992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f49a1c397b4a9cdc0f9a6cd1eb6aea12154952a3d4ead09ddd6c9595bb4361`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:43:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Dec 2020 02:43:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 11 Dec 2020 02:43:33 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 11 Dec 2020 02:43:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Dec 2020 02:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:43:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Dec 2020 02:43:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/config]
# Fri, 11 Dec 2020 02:43:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Fri, 11 Dec 2020 02:43:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Dec 2020 02:43:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Dec 2020 02:43:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Dec 2020 02:43:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 80
# Fri, 11 Dec 2020 02:43:49 GMT
EXPOSE 443
# Fri, 11 Dec 2020 02:43:50 GMT
EXPOSE 2019
# Fri, 11 Dec 2020 02:43:50 GMT
WORKDIR /srv
# Fri, 11 Dec 2020 02:43:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7871a798b8122182b3e65559fefc21812c1f2c881d60555d71c1353136d54`  
		Last Modified: Fri, 11 Dec 2020 02:44:24 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752f95e37b35ec8cf81bd3caab7ba2ea836620747fa2d720c5b64709254ddae`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f574024c894c439da18a68fa9e20ef03be94dd77a2b1934242463f93d518b0`  
		Last Modified: Fri, 11 Dec 2020 02:44:34 GMT  
		Size: 11.2 MB (11202556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26947b55683beda16dec6f01fc3ef037d91c61349dae0527952bafce3c03d5c0`  
		Last Modified: Fri, 11 Dec 2020 02:44:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:94222b11fa710228c495d0963ae695e54d8e8e5ef631517a00f7e2557465e82e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:6f9fa402f617af6a08a77a3d6821621bb5bb0f3b99080d2d9b8d990104a3fb48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull caddy@sha256:b99f350b2de1665d145dad8c93c867427211ed43e1676b25da7c573bf24e97cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416743592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:242dc82d58b3eb28bad3e05fe3004a6da6c5748d32c08be14523fcafd480cbc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:50:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:50:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:51:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:51:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:51:17 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:51:18 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:51:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:51:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:51:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:51:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:51:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:51:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:51:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:51:25 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:51:26 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:51:27 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:51:43 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:51:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433ced4e59cd32da7d04608be235ec50650c9160c8742a10c9a60ae7294d7f52`  
		Last Modified: Wed, 09 Dec 2020 22:59:41 GMT  
		Size: 9.2 MB (9243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914209fee7eb59b47ff4c4135d33f98b6b3af4209d114af2f9d0a8f65849d39b`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493568bf34f325205007ec539e481c37dd13dd690c9e40e265f5a985393ba1a2`  
		Last Modified: Wed, 09 Dec 2020 22:59:43 GMT  
		Size: 16.3 MB (16325951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee88af8a1f1057877ee81813d03ca89698521e3a410830835be694de9aa3153`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bfb8247c1f8c75fb59ee12dcd363fd2fcae2ac8da5e9fede5617faec7d082c`  
		Last Modified: Wed, 09 Dec 2020 22:59:37 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326e317e6021cafd340d9cb540564d2c79890682efe4baa10fe5bea17847adba`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3769dc06e616a825c947d4d1a6c8aa5a427cf792adea55a9dc35672cc76b6d6`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa4f4d0eb978c7b41fb792c1faf3fc4823a131abc37ca7de8f13f2cb6b56d8`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1042475d4dc01a2523d8dae43fd2096a6b87435d2f47f8c3275fcbac6d2453b`  
		Last Modified: Wed, 09 Dec 2020 22:59:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f1d1c1053e1fb4775c5939504f7c7554f3c65d033668836428b399f7bd3269`  
		Last Modified: Wed, 09 Dec 2020 22:59:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4951dcfb5db6ad1ce8c0778b1647a8950ced04bd7b2b3051bf2b9df7209a4`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dc0af1dcce3f75d580aaa3f73c92c6bd81249b0e86db979abe8ab511744095`  
		Last Modified: Wed, 09 Dec 2020 22:59:32 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c49ff4855aff0e5bec5047249790dc3beef9bb99303c7963e0060e19c781e`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db82d6aa5350a637ef41ced50f1e2aaab1876acadc50f289261c2b935251abda`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ca7f7662411153b8d2e07b4e190fe5f28b55987e6c488eaf407f1b218757db`  
		Last Modified: Wed, 09 Dec 2020 22:59:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08ddd6fa1eec7ccc22299391dd16977f04c771c608d78aac09c2001b65cf36`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11252ce2cac0c2d7e62754856c25a1fff65491437f664d589da9d70b608b18c4`  
		Last Modified: Wed, 09 Dec 2020 22:59:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159813c0e3aae77d0d2682fc6af3e2efa7204512c729017ee3c3282ba2a0ef30`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a54bb1a8f7a905eb1774d7a6343ba5d306106c5dea74d1c9bd6e501cadcc86`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 279.4 KB (279413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326eaebe45d7e1cadffa1215c3c58ff62541eba9a6209d0140f165099ca8d66b`  
		Last Modified: Wed, 09 Dec 2020 22:59:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:358936d5db6ea416ac9bd28395c579cf0f12fe0f53065eff3dd7a6e1ec101ecb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull caddy@sha256:690a9e8ed59ad073fdf48712bad9bb8a3c942d100c4b379b3f01895905dada9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800848400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15cdc648fca30457ce53eff362d47ce02aebefe3e3869c7a67003cc9f3de197`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 22:53:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Dec 2020 22:53:09 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 09 Dec 2020 22:54:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Dec 2020 22:54:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Dec 2020 22:54:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/config]
# Wed, 09 Dec 2020 22:54:30 GMT
VOLUME [c:/data]
# Wed, 09 Dec 2020 22:54:31 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 09 Dec 2020 22:54:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Dec 2020 22:54:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Dec 2020 22:54:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Dec 2020 22:54:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Dec 2020 22:54:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 80
# Wed, 09 Dec 2020 22:54:37 GMT
EXPOSE 443
# Wed, 09 Dec 2020 22:54:38 GMT
EXPOSE 2019
# Wed, 09 Dec 2020 22:55:19 GMT
RUN caddy version
# Wed, 09 Dec 2020 22:55:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d43cde540577a280266a838cfa13afe6a9cc3f995da2c60a9edbe76f85fc2`  
		Last Modified: Wed, 09 Dec 2020 23:00:17 GMT  
		Size: 10.1 MB (10058208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1cb3aba27a86c6bfc96c6ee8f1778fc34c803d6a73e028b772f353bdaa1920`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba08ee40b5c7cc6bd794314039785636c387c33b03b6ae8804c82855546d4e`  
		Last Modified: Wed, 09 Dec 2020 23:00:19 GMT  
		Size: 21.7 MB (21688147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6bf11341a084f6e721ab3307d585db365feab3cafe5ccd13d3e45eaa825b6b`  
		Last Modified: Wed, 09 Dec 2020 23:00:12 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5652f1edbffbb90424a031a590be746b88955531f465e3171071cc861627cfdb`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5879654d1ba873fbefe4d4f4cf04f4fc236c1b06355739aace87094aec7a247`  
		Last Modified: Wed, 09 Dec 2020 23:00:10 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7249d7e148d894abc47de261d624f605c263a6c5d33f946ab44cbf8508e801`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f17c7f16448f909172bb4ab2387cb8a9fbe53015f31945a485281b6780770`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2518f043ac15f96f3d7209cd9ba09a011801e4893ee20b93e997894a7d05c`  
		Last Modified: Wed, 09 Dec 2020 23:00:09 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea0ee4a2384e36d3d715826e698e92ad2973d37760c3739c7f24c1d5b6e5630`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a728aa2135880e4bda604c4f3dda7a805432c5020dcc5caa91cbca2bb1c1ebda`  
		Last Modified: Wed, 09 Dec 2020 23:00:06 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce4a1edefa2c1d049421764a2d56c2b6698f59cfeabcee1650f49af3a411c7`  
		Last Modified: Wed, 09 Dec 2020 23:00:07 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544505e4f2dca7871e19f148b8e5b0fcda661f26231146305a4117953193d15`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e367b8829addd164fd7523883f9a4afaac2a45f397996f9f555dfc9f9efc787`  
		Last Modified: Wed, 09 Dec 2020 23:00:05 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f338885dde1e48da16a2adea5f227ea93400f0bba92c5b26c19ce6c5ffdee`  
		Last Modified: Wed, 09 Dec 2020 23:00:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34fec3499c9069ad73d1134ff56ae4bcfd60f542595684ffb5aab21094eaed8`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9193a0ae2298ef7b30b475844d6b0ceafade168d507d7e310b8b5224461bf108`  
		Last Modified: Wed, 09 Dec 2020 23:00:01 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729f45a6315ae599187516f7d0dfbb7d855407b87648a38e0a53b4804f5cb319`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9db07c0857db2b49c14d6c4dd764126c4945a573a5a3edb3b0278465f741c8`  
		Last Modified: Wed, 09 Dec 2020 23:00:03 GMT  
		Size: 238.3 KB (238322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b684f9fb9937abcabf60ad70959f5344b4721c043ec4fa2cf21864d7af779`  
		Last Modified: Wed, 09 Dec 2020 23:00:02 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
