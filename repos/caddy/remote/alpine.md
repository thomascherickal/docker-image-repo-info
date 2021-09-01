## `caddy:alpine`

```console
$ docker pull caddy@sha256:a6e9d4eb7ef61a4fefbe1242f13ba025988f140ffa3be38c9830167e4973f1b4
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
$ docker pull caddy@sha256:f9c6cd548d4604bdd74b3f8f41ed9342d0d059f18339197d9bf304950170ed28
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14650310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcef364d05b843db86f14bd39f79653a9ef3e6172a32486e3eca981b4644d35`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:22:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 01 Sep 2021 00:22:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 01 Sep 2021 00:22:15 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 01 Sep 2021 00:22:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Sep 2021 00:22:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:22:21 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Sep 2021 00:22:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Sep 2021 00:22:22 GMT
VOLUME [/config]
# Wed, 01 Sep 2021 00:22:22 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 00:22:22 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 01 Sep 2021 00:22:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Sep 2021 00:22:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Sep 2021 00:22:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Sep 2021 00:22:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Sep 2021 00:22:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Sep 2021 00:22:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Sep 2021 00:22:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Sep 2021 00:22:25 GMT
EXPOSE 80
# Wed, 01 Sep 2021 00:22:25 GMT
EXPOSE 443
# Wed, 01 Sep 2021 00:22:26 GMT
EXPOSE 2019
# Wed, 01 Sep 2021 00:22:26 GMT
WORKDIR /srv
# Wed, 01 Sep 2021 00:22:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b89ea1812e905dc789434abfd657abb284a217e64dc1e1d7b883f650b4c272`  
		Last Modified: Wed, 01 Sep 2021 00:22:59 GMT  
		Size: 300.4 KB (300409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7af07c25c26d1f7bd2565b33853ca26558d164310e140d65e72aed5c7e2c65`  
		Last Modified: Wed, 01 Sep 2021 00:22:59 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a97be68bcca30ca461d850134337a5f4d564e3b37c787f2d0f9c0b2e7e77c2`  
		Last Modified: Wed, 01 Sep 2021 00:23:02 GMT  
		Size: 11.5 MB (11529818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b1748c7f9267ab8160ec6dab3c793cba9b3c5a09749a02f2859339d4e69f8e`  
		Last Modified: Wed, 01 Sep 2021 00:23:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:499ba0ef68cd17c87d19ad475c7c388e739d114e5aafbed7420ec6fa749cba9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13818222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91ab7dd1223f81f381df8605f8b1d4ba06aa4f8b53294bcf82037eefb0dc15af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 01 Sep 2021 01:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 01 Sep 2021 01:21:19 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 01 Sep 2021 01:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Sep 2021 01:21:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 01:21:25 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Sep 2021 01:21:26 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Sep 2021 01:21:26 GMT
VOLUME [/config]
# Wed, 01 Sep 2021 01:21:27 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 01:21:27 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 01 Sep 2021 01:21:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Sep 2021 01:21:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Sep 2021 01:21:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Sep 2021 01:21:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Sep 2021 01:21:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Sep 2021 01:21:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Sep 2021 01:21:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Sep 2021 01:21:31 GMT
EXPOSE 80
# Wed, 01 Sep 2021 01:21:31 GMT
EXPOSE 443
# Wed, 01 Sep 2021 01:21:31 GMT
EXPOSE 2019
# Wed, 01 Sep 2021 01:21:32 GMT
WORKDIR /srv
# Wed, 01 Sep 2021 01:21:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a409db32a02a241c3193afe4db6821448699a7961379585dcf440b4088e11a7`  
		Last Modified: Wed, 01 Sep 2021 01:22:48 GMT  
		Size: 300.5 KB (300514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7ade09f320de7f91d1565fc7843a9c10b33d0a257626cdb39004f43a7971da`  
		Last Modified: Wed, 01 Sep 2021 01:22:47 GMT  
		Size: 5.8 KB (5849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fa31fa9a55504a09b104fa0d316535dd6b00882242aa315d65293a6c2668ec`  
		Last Modified: Wed, 01 Sep 2021 01:22:55 GMT  
		Size: 10.9 MB (10887945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ab5ffbc60bd19e1c16558d377d597985bf28300cb2e82945331fd3b55ec6a4`  
		Last Modified: Wed, 01 Sep 2021 01:22:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c382c62559cf6348cccc2048f7f6e3234ad6c3322fa778f0d7ab3fbe27cd44e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c6676bf8617209d68af4cbdd3c3edb6084cbd01e6c7f00b706fab8934f311a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Fri, 30 Jul 2021 18:36:39 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 02:13:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 31 Jul 2021 02:13:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 31 Jul 2021 02:13:44 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 31 Jul 2021 02:13:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 31 Jul 2021 02:13:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 31 Jul 2021 02:13:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 31 Jul 2021 02:13:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 31 Jul 2021 02:13:52 GMT
VOLUME [/config]
# Sat, 31 Jul 2021 02:13:52 GMT
VOLUME [/data]
# Sat, 31 Jul 2021 02:13:53 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 31 Jul 2021 02:13:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 31 Jul 2021 02:13:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 31 Jul 2021 02:13:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 31 Jul 2021 02:13:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 31 Jul 2021 02:13:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 31 Jul 2021 02:13:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 31 Jul 2021 02:13:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 31 Jul 2021 02:13:56 GMT
EXPOSE 80
# Sat, 31 Jul 2021 02:13:57 GMT
EXPOSE 443
# Sat, 31 Jul 2021 02:13:57 GMT
EXPOSE 2019
# Sat, 31 Jul 2021 02:13:58 GMT
WORKDIR /srv
# Sat, 31 Jul 2021 02:13:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bf509b321d9275e96242772f4cd73ad8da2970e30e18c0f2326ed91777442e`  
		Last Modified: Sat, 31 Jul 2021 02:15:13 GMT  
		Size: 299.7 KB (299672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16416239cfcd26ea4cc02aaf7ac5511b6ea5d6cc672046b6e61d90f9c59ffaac`  
		Last Modified: Sat, 31 Jul 2021 02:15:13 GMT  
		Size: 5.9 KB (5854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de14f3facde68cf2e2470839f96bb111537c6b40d15a1b28c47c6568261ee15`  
		Last Modified: Sat, 31 Jul 2021 02:15:20 GMT  
		Size: 10.9 MB (10863669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b241bda44fe422ccd7c0c967fb01d2d7a191df7b0628d9c44df2d18dd5445`  
		Last Modified: Sat, 31 Jul 2021 02:15:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
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
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
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
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:fff2119338c215eceae68398483da801f5daf8bb5405c7ed8db5769aeb367cd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced11b632073f0e249ba02b8326f0c1ccf6c154d4340342b38c8b3f830c37e70`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:49 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Fri, 30 Jul 2021 17:24:54 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 00:36:43 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 31 Jul 2021 00:36:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 31 Jul 2021 00:36:54 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 31 Jul 2021 00:37:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 31 Jul 2021 00:37:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 31 Jul 2021 00:37:12 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 31 Jul 2021 00:37:14 GMT
ENV XDG_DATA_HOME=/data
# Sat, 31 Jul 2021 00:37:17 GMT
VOLUME [/config]
# Sat, 31 Jul 2021 00:37:23 GMT
VOLUME [/data]
# Sat, 31 Jul 2021 00:37:27 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 31 Jul 2021 00:37:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 31 Jul 2021 00:37:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 31 Jul 2021 00:37:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 31 Jul 2021 00:37:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 31 Jul 2021 00:37:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 31 Jul 2021 00:37:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 31 Jul 2021 00:38:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 31 Jul 2021 00:38:06 GMT
EXPOSE 80
# Sat, 31 Jul 2021 00:38:09 GMT
EXPOSE 443
# Sat, 31 Jul 2021 00:38:16 GMT
EXPOSE 2019
# Sat, 31 Jul 2021 00:38:25 GMT
WORKDIR /srv
# Sat, 31 Jul 2021 00:38:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ee5e0a948db1cebd77a9b357abbc39c60dc4caf97f87f759a1f232a291da5`  
		Last Modified: Sat, 31 Jul 2021 00:39:14 GMT  
		Size: 302.5 KB (302545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c405a506bbc65ab625ac9298a31abc4a1871eef7b93ff4fbc6a25fb9db591a4`  
		Last Modified: Sat, 31 Jul 2021 00:39:14 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac195b709078a7d439cd22a970947cb2ed3f9cd136a8d51324ab3d3c746625`  
		Last Modified: Sat, 31 Jul 2021 00:39:16 GMT  
		Size: 10.1 MB (10051943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2c9f1da5ba05b5656393520168363c5d8a223167645bc0a4451fcd4c2f5447`  
		Last Modified: Sat, 31 Jul 2021 00:39:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:576d8d6d9dead63f0cc0db39ad0fb1e9e9539bf5b23a8b70623b7e8f40d916a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6114aef9a435617ae101cc26569f3f2103cd2c999ef3e41df780270222452a1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 30 Jul 2021 17:41:41 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Fri, 30 Jul 2021 17:41:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Jul 2021 23:50:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 30 Jul 2021 23:50:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 30 Jul 2021 23:50:46 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 30 Jul 2021 23:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 30 Jul 2021 23:50:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 30 Jul 2021 23:50:49 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 30 Jul 2021 23:50:49 GMT
ENV XDG_DATA_HOME=/data
# Fri, 30 Jul 2021 23:50:50 GMT
VOLUME [/config]
# Fri, 30 Jul 2021 23:50:50 GMT
VOLUME [/data]
# Fri, 30 Jul 2021 23:50:50 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 30 Jul 2021 23:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 30 Jul 2021 23:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 30 Jul 2021 23:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 30 Jul 2021 23:50:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 30 Jul 2021 23:50:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 30 Jul 2021 23:50:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 30 Jul 2021 23:50:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 30 Jul 2021 23:50:52 GMT
EXPOSE 80
# Fri, 30 Jul 2021 23:50:52 GMT
EXPOSE 443
# Fri, 30 Jul 2021 23:50:52 GMT
EXPOSE 2019
# Fri, 30 Jul 2021 23:50:52 GMT
WORKDIR /srv
# Fri, 30 Jul 2021 23:50:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de364003ff53d3ed839a7d8fd8cc6c59936d04b22886595d954e5c9929cfe0e1`  
		Last Modified: Fri, 30 Jul 2021 23:51:32 GMT  
		Size: 300.9 KB (300858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d9b83bb28f1c9bc97f9a4907425be62b28dd687b54e3b8d461b2e40203110d`  
		Last Modified: Fri, 30 Jul 2021 23:51:32 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076584d90c472ad966977bc9f55f53439edb7b5169fa684c1a70a1ea682037ca`  
		Last Modified: Fri, 30 Jul 2021 23:51:34 GMT  
		Size: 11.1 MB (11096451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f126f1c964e9405478f4683dd4b8e93297166d84566a652fe658f36bad6390c`  
		Last Modified: Fri, 30 Jul 2021 23:51:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
