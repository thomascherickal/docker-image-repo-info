## `caddy:alpine`

```console
$ docker pull caddy@sha256:8b9b0db50cc8e8a39439cf98d68b338428f59ace5bf2ad8f22e0a3d19dd54b61
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
$ docker pull caddy@sha256:1bdf3e5038d669d4c7beeaa17b792942c5fe642b3a8af6f25121d7ba3e12f9c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13594720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c31b1758fe22898471d7d084b655234263459738efef18c26015b6d24674c71`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 01 Sep 2021 01:26:54 GMT
ADD file:4a3cd5b6e6a9e76edf236ec86eb493ae8b09bf3220a8c0fdcaa474b9d6135ad3 in / 
# Wed, 01 Sep 2021 01:26:55 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 10:25:33 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 01 Sep 2021 10:25:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 01 Sep 2021 10:25:36 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 01 Sep 2021 10:25:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Sep 2021 10:25:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 10:25:43 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Sep 2021 10:25:43 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Sep 2021 10:25:43 GMT
VOLUME [/config]
# Wed, 01 Sep 2021 10:25:44 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 10:25:44 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 01 Sep 2021 10:25:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Sep 2021 10:25:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Sep 2021 10:25:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Sep 2021 10:25:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Sep 2021 10:25:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Sep 2021 10:25:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Sep 2021 10:25:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Sep 2021 10:25:48 GMT
EXPOSE 80
# Wed, 01 Sep 2021 10:25:48 GMT
EXPOSE 443
# Wed, 01 Sep 2021 10:25:49 GMT
EXPOSE 2019
# Wed, 01 Sep 2021 10:25:49 GMT
WORKDIR /srv
# Wed, 01 Sep 2021 10:25:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:48fad15491f9799a77d01e4a4a3b0e201ca2aba6f0849c39afa1160d6f3d905a`  
		Last Modified: Wed, 01 Sep 2021 01:28:39 GMT  
		Size: 2.4 MB (2425373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc2338a417300f64aa44292d38440bb9847efda48333a6cf8d6d3445d55be25`  
		Last Modified: Wed, 01 Sep 2021 10:27:07 GMT  
		Size: 299.7 KB (299668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b9b4af9f8c402b7426290c9be0794eb38f372f44b793ea6f208215808985c3`  
		Last Modified: Wed, 01 Sep 2021 10:27:07 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f99ede116bae02957470c70816c62a29b4566aa8416274add1c23665e0c45f`  
		Last Modified: Wed, 01 Sep 2021 10:27:14 GMT  
		Size: 10.9 MB (10863675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2170b602e6278020bc3bf55325a979d58793df6e4a033eba30b6ecb1e4524d`  
		Last Modified: Wed, 01 Sep 2021 10:27:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7f54a972333e4a76679da47353106d9201fba82f84692b50829d7583a7c10e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13465740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf7e12f71e00eb9b1e840d0a2f19360fb9f38d85c03fe0b79b9800b6580d2e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:36:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 01 Sep 2021 11:36:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 01 Sep 2021 11:36:47 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 01 Sep 2021 11:36:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Sep 2021 11:36:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 11:36:49 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Sep 2021 11:36:50 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Sep 2021 11:36:50 GMT
VOLUME [/config]
# Wed, 01 Sep 2021 11:36:50 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 11:36:50 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 01 Sep 2021 11:36:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Sep 2021 11:36:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Sep 2021 11:36:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Sep 2021 11:36:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Sep 2021 11:36:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Sep 2021 11:36:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Sep 2021 11:36:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Sep 2021 11:36:52 GMT
EXPOSE 80
# Wed, 01 Sep 2021 11:36:52 GMT
EXPOSE 443
# Wed, 01 Sep 2021 11:36:52 GMT
EXPOSE 2019
# Wed, 01 Sep 2021 11:36:52 GMT
WORKDIR /srv
# Wed, 01 Sep 2021 11:36:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35341aa316d90f4035f5a01628c5897c280bd9d6a52348c96cc288d38f7833af`  
		Last Modified: Wed, 01 Sep 2021 11:37:32 GMT  
		Size: 300.6 KB (300632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573dfae7b0d35d76130c61f612a28770d3822153f2c804fcb44a3f0d236b2a79`  
		Last Modified: Wed, 01 Sep 2021 11:37:31 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ac67fabb9cb29395e8ac7adc346e26c607a8b1e74c79a0526d68fc3a1eef`  
		Last Modified: Wed, 01 Sep 2021 11:37:33 GMT  
		Size: 10.4 MB (10446105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea6ddbd4c2f04df35c34617c3419d26a86384195e0de6a6e16895ad9a384260`  
		Last Modified: Wed, 01 Sep 2021 11:37:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:92379d4bccf3f5eeacd0e2e357c8f0e625b1d757ac07d32aa762996c4461e06d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4595760a15c4eb11cce97da592b99b503c7cb391a3469a2fb8def408f164d8d7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:15:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 01 Sep 2021 11:16:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Wed, 01 Sep 2021 11:16:08 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 01 Sep 2021 11:16:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Sep 2021 11:16:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 11:16:25 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Sep 2021 11:16:27 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Sep 2021 11:16:30 GMT
VOLUME [/config]
# Wed, 01 Sep 2021 11:16:34 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 11:16:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 01 Sep 2021 11:16:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Sep 2021 11:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Sep 2021 11:16:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Sep 2021 11:16:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Sep 2021 11:16:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Sep 2021 11:16:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Sep 2021 11:17:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Sep 2021 11:17:15 GMT
EXPOSE 80
# Wed, 01 Sep 2021 11:17:23 GMT
EXPOSE 443
# Wed, 01 Sep 2021 11:17:26 GMT
EXPOSE 2019
# Wed, 01 Sep 2021 11:17:32 GMT
WORKDIR /srv
# Wed, 01 Sep 2021 11:17:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d20bb0ddf404db9ff36b42ae7f1807c3dd9666c6bc029b424f13cb2047f6ba`  
		Last Modified: Wed, 01 Sep 2021 11:18:32 GMT  
		Size: 302.5 KB (302545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d05c52d55fdba14a84abe37ed05b8a8e62c951ca110210cc7a11411cb1eb649`  
		Last Modified: Wed, 01 Sep 2021 11:18:32 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f5d794ae71261091c4b815fc2b3361123fe01b39f0415f7e97c60365df600b`  
		Last Modified: Wed, 01 Sep 2021 11:18:34 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57da93899e277b7eae14381772a9fd8383bd2da5111bf71e977946e17a327281`  
		Last Modified: Wed, 01 Sep 2021 11:18:32 GMT  
		Size: 155.0 B  
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
