## `caddy:alpine`

```console
$ docker pull caddy@sha256:2a518987da6ad50fba4fa2ce40b159460bc68d42e4d37c7784c118470e738821
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
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 17:34:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 17:34:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c2672622a603ff8b0ed8517cfd5adb30b2b35ae40b42cd4ad0545dcb6d3b10`  
		Last Modified: Wed, 26 May 2021 17:36:11 GMT  
		Size: 300.5 KB (300528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b30604f35cc25a62ae1d71a50c6919ad28a2aa67bfd14bebc1984cec5b2c8b`  
		Last Modified: Wed, 26 May 2021 17:36:12 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 10:59:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 May 2021 10:59:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca051a8c4175c3d7d75c47c9a60045d2f5b7eb415ce35b56c99e9cab58ae3ba`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db810fb832f7bd380a39ff7508fa03cc1854bdd51da4cfa239e07fe96fe4e`  
		Last Modified: Wed, 26 May 2021 11:01:09 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
