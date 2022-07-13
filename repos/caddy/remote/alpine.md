## `caddy:alpine`

```console
$ docker pull caddy@sha256:770022ce91e8dfab5ffef6bc37fff243ff83bf911d5d3a0c38783cb5fa88fb96
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
$ docker pull caddy@sha256:2e61a3ed70ad9a4784ff95cf49efa7ec58255c5263c3faba6a5270a847542a41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15835582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c6db987e0721fcd4f557ec160b55012a73d2f69de7198fac316514b27ed58f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:57:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:57:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:57:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:57:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:57:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:57:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:57:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:57:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 80
# Fri, 06 May 2022 19:57:43 GMT
EXPOSE 443
# Fri, 06 May 2022 19:57:44 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:57:44 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:57:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507adf96fcab6911303d2b3d14aeb43223c106ee9901b3e31f30668a4dbd5ffb`  
		Last Modified: Fri, 06 May 2022 19:59:02 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435dc592c99e66d2e9f715136b809e73116ee6725847ed8fd158135e3283be`  
		Last Modified: Fri, 06 May 2022 19:59:11 GMT  
		Size: 13.1 MB (13114610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e55b7a8b43f4fdfecf61cea01ddddc80930ed485d9aafc41c26f84380f858f3`  
		Last Modified: Fri, 06 May 2022 19:59:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:cda45585c425161575996ee5d954166745d44d39928846423ecdce6b61a9fb4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15523770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cdb4fef0cc66aabb117ff1b3e11fb86de5117d28a5b0e64a743efb92c4269`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:39:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:39:32 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:39:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:39:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:39:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:39:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:39:39 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:39:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:39:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:39:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:39:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:39:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:39:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:39:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:39:47 GMT
EXPOSE 80
# Fri, 06 May 2022 19:39:48 GMT
EXPOSE 443
# Fri, 06 May 2022 19:39:49 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:39:50 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:39:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc050d3d6ffb91c2f68db47e3d5f056afad26e465a03ae7e43383df0fc8ad89`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adaff0bd78d0b115843dd841c83d1690484b25369e804b1133b838b7ad5ce8f`  
		Last Modified: Fri, 06 May 2022 19:40:35 GMT  
		Size: 12.5 MB (12510086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703c61da5ec8e48b081aceac2cb64fb25162c2f0ba1ad16a104610b676f50f6`  
		Last Modified: Fri, 06 May 2022 19:40:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d1ab9f3165d5b23b9ff5bd4fcb74b3f8bbf834ba34c42c58e496b3d33017ca59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15203958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbb2004b1ba3aace5176af38455ef6b8328a074388b16b35358d61330ad2658`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:16:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:16:58 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:17:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:17:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:17:25 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:17:32 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:17:36 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:17:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:17:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:17:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:17:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:17:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:18:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:18:13 GMT
EXPOSE 80
# Fri, 06 May 2022 19:18:17 GMT
EXPOSE 443
# Fri, 06 May 2022 19:18:19 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:18:22 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:18:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b659dd8890d066269209696348c58ed19351199266936a5e81f1991a52333d1`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86272ae554176010d052c51dcc5540948b8e59082743b04ac5bb67d05c3fdcd`  
		Last Modified: Fri, 06 May 2022 19:19:33 GMT  
		Size: 12.1 MB (12093067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57ff409904cc43937df14c68e6d97e1269adde095e91671fb5438dc58a1808`  
		Last Modified: Fri, 06 May 2022 19:19:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:fbee089e769bc54babbe3ac3217c0e5b60c4a5157b76b0f37aa73cc71486c8fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16129299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94fa793c943e1cb1c5bda77b0e7077b344648635da2222a1061307e3e61ca96`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 06 May 2022 19:41:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/69bb1c539b3ee03fc91271a71653a77ca1e9d131/welcome/index.html"
# Fri, 06 May 2022 19:41:25 GMT
ENV CADDY_VERSION=v2.5.1
# Fri, 06 May 2022 19:41:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2e4903c04f1918710566d5bca2b7b7ed6e8319aa925275040a9d9af87198cbc202b1f76b8ce0282f4423da9afb8634a14b59dd420879a188d024c5cbcf32b771' ;; 		armhf)   binArch='armv6'; checksum='93648db05fabddb8b284d952895be26700908bcd3d3a4102529dc8ca9365c11e942672b9b19b64a4ed0b08880410b388f4c89276bf83e5dd77a7c4c5049c1619' ;; 		armv7)   binArch='armv7'; checksum='ada8f06d71c088e8f6cf872c427710ae236a44cb8f18c4b0ba58663f49db8beb7a5caee18d0b23bd67a8db94fd839e5273ff9cd1b928576b4748072279cfb335' ;; 		aarch64) binArch='arm64'; checksum='33421b53b12d642f2439321cd6bb6b72e93a5585601febad051b461cfe5cac09a983ce8b2f60bc8b045ee2a583e53ce1d595123f14f4bf6ea07c5c4da07b6465' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='bcd738433a37d5f5a47ed668ae517adbef5cb3aa406d1e449d6ea7eb077de4c85bfb199490929d97fb3c5d1edef40d49d1a7f080f8972e5a606f783362facb24' ;; 		s390x)   binArch='s390x'; checksum='bbeb8f6e6f9dadb306e4d73f85ada7cc2c2e1d3e29ef6db16b19bef915681c83f145bf96cd9ac2f1c4d551b7a25be5c9b9c642b59136ecdb08d77b2a3a081f37' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.1/caddy_2.5.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 06 May 2022 19:41:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 06 May 2022 19:41:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.version=v2.5.1
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 80
# Fri, 06 May 2022 19:41:29 GMT
EXPOSE 443
# Fri, 06 May 2022 19:41:30 GMT
EXPOSE 2019
# Fri, 06 May 2022 19:41:30 GMT
WORKDIR /srv
# Fri, 06 May 2022 19:41:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d2fae470dbad90c4c4c1262110f14447a47b6e81edc4e0e80ceb50538fe57`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8f9dbbf38ad9456666a4e6a3eda871b385d4ef76ab6dc25e31030d1daf71c`  
		Last Modified: Fri, 06 May 2022 19:42:12 GMT  
		Size: 13.2 MB (13231118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf07e991258bc58c5e8a5785f741bc746e75848423d2c27d26448015c5887f1`  
		Last Modified: Fri, 06 May 2022 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
