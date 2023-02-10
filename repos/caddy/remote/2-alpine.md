## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:08f253f077fb51f188959adb024b5816903d8302af018fb26956308a1f0a2781
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
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a12f8b257edf723252fe4d7904cd7da6427f0143cd91fd8f1c66d4238d8fc3b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16360408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e339ad4e3cdbcdb2b56b0f159d20385f1b8ba9df46bd139c4648267b3ed55454`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Wed, 08 Feb 2023 23:57:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Feb 2023 23:57:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Feb 2023 23:57:29 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Feb 2023 23:57:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Feb 2023 23:57:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Feb 2023 23:57:32 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Wed, 08 Feb 2023 23:57:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Feb 2023 23:57:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 80
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 443
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 443/udp
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 2019
# Wed, 08 Feb 2023 23:57:34 GMT
WORKDIR /srv
# Wed, 08 Feb 2023 23:57:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a12332fdf16ce73aea4764330485716ca48d192a121a2fd401dc2c0b39218f`  
		Last Modified: Wed, 08 Feb 2023 23:58:28 GMT  
		Size: 342.6 KB (342593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b77a300a01493d7a60c76bceedba787157bd56b11597beb662bdb689c2ad2a`  
		Last Modified: Wed, 08 Feb 2023 23:58:28 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79d8027362d8d140a1b1f357f0eeb8db4538ad6953141f1be740c8f251f1f7`  
		Last Modified: Wed, 08 Feb 2023 23:58:31 GMT  
		Size: 13.6 MB (13591547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
