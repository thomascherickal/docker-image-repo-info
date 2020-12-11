## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:92e4315d32463e7fdd83fe17ddac62cfb128423a9dcdc34deca64e6f2d7759cc
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
$ docker pull caddy@sha256:09208042b4d19d7ed87b51b99dc20b390dab20d9ae7e235a62a3af3aaf472bd5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13291756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5c77284adc35481d13003d31a866f637b6eaf9f5764f667e536db79ce23129`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 13:39:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 22 Oct 2020 13:44:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 22 Oct 2020 13:44:04 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 22 Oct 2020 13:44:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Oct 2020 13:44:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 13:44:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Oct 2020 13:44:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Oct 2020 13:44:40 GMT
VOLUME [/config]
# Thu, 22 Oct 2020 13:44:44 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 13:44:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 22 Oct 2020 13:44:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Oct 2020 13:44:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Oct 2020 13:45:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Oct 2020 13:45:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Oct 2020 13:45:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Oct 2020 13:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Oct 2020 13:45:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Oct 2020 13:45:23 GMT
EXPOSE 80
# Thu, 22 Oct 2020 13:45:26 GMT
EXPOSE 443
# Thu, 22 Oct 2020 13:45:30 GMT
EXPOSE 2019
# Thu, 22 Oct 2020 13:45:35 GMT
WORKDIR /srv
# Thu, 22 Oct 2020 13:45:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a4964211b7ce86541a0c1dad8ef3800ec38a3ca90aff94b76759b4cb8e279`  
		Last Modified: Thu, 22 Oct 2020 13:47:22 GMT  
		Size: 302.3 KB (302327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dd938ef3e3eae8509deda8fab9ab5f9344169d912e35a802633e799feed1bb`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23c296ee12ee12ef84dbabbb4f7bf0362a9a12b684782ebd3f44a97c8fcf8e`  
		Last Modified: Thu, 22 Oct 2020 13:47:55 GMT  
		Size: 10.2 MB (10180223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2f3c084745fecafaa9ff33626a81124f2d70267ceee705da555714238bfa1`  
		Last Modified: Thu, 22 Oct 2020 13:47:52 GMT  
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
