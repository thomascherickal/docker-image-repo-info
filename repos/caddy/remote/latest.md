## `caddy:latest`

```console
$ docker pull caddy@sha256:1c4a1e06e0d3e96fc1b5becd8032664c2cc891f72d2838d4af600802a4f9d6a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fe42da7df688686dab79fb02be7f13aae32c9a9f84eec3b28b634cc48d5a7346
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f95b690a9e892f56dbf3fd455d714c2d22ebd35967fdc770fb704c870eeffc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 08 Dec 2023 20:07:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/welcome/index.html"
# Fri, 08 Dec 2023 20:07:47 GMT
ENV CADDY_VERSION=v2.7.6
# Fri, 08 Dec 2023 20:07:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b74311ec8263f30f6d36e5c8be151e8bc092b377789a55300d5671238b9043de5bd6db2bcefae32aa1e6fe94c47bbf02982c44a7871e5777b2596fdb20907cbf' ;; 		armhf)   binArch='armv6'; checksum='88756642ca412db3a8da7a40b518861a6f524a8ac704021e8451d3cb38746f24243b1e561f4eec07e1575200d06bfd098783d2b7ee7ee07a971aed1c677da6e6' ;; 		armv7)   binArch='armv7'; checksum='118776e879c280556abb7c03ff7c0081eda23c2aee0472aef176f733785e9501defaeaf334cd2443e31294809beafaea831d2e695aa68045160082aa3a966e2f' ;; 		aarch64) binArch='arm64'; checksum='62252ade5e8dcec13a66154ee1978d959370be049cce52e7c4edefff14ef70bbb21630e3735092719bc3c31214e89dff99e55970ff0adec8ac0a94c6415b059a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='65d27fe53f5e4fa79f3476f8902071c907aab74db1a2616342be3714d4252219fbb53b174ef588e20c51e7cfac84376c7a0a608091c2fe83b31dbf59dabeb237' ;; 		s390x)   binArch='s390x'; checksum='c562190962a2db0248a4190616dd2ebaa02df2cf62f1a2c71f9d9de18af2a297df8000a06a11e8d3929dfd64f0c081d1e61961687ca220007459f2dbd0be2c81' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.6/caddy_2.7.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 08 Dec 2023 20:07:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 08 Dec 2023 20:07:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 08 Dec 2023 20:07:50 GMT
LABEL org.opencontainers.image.version=v2.7.6
# Fri, 08 Dec 2023 20:07:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 08 Dec 2023 20:07:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 08 Dec 2023 20:07:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 08 Dec 2023 20:07:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 08 Dec 2023 20:07:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 08 Dec 2023 20:07:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 08 Dec 2023 20:07:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 08 Dec 2023 20:07:51 GMT
EXPOSE 80
# Fri, 08 Dec 2023 20:07:51 GMT
EXPOSE 443
# Fri, 08 Dec 2023 20:07:51 GMT
EXPOSE 443/udp
# Fri, 08 Dec 2023 20:07:51 GMT
EXPOSE 2019
# Fri, 08 Dec 2023 20:07:51 GMT
WORKDIR /srv
# Fri, 08 Dec 2023 20:07:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1775b4c8558ad1bf8d7568fc741be39ee2a28ecdd33f84ed7597b6192873a81a`  
		Last Modified: Fri, 08 Dec 2023 20:08:10 GMT  
		Size: 7.5 KB (7529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf57a0db316ab6b42386b0221d652cc4f9d9d597206ce1d4e9bfd5ba0f7777`  
		Last Modified: Fri, 08 Dec 2023 20:08:12 GMT  
		Size: 13.9 MB (13920999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:71069b6f75345cd8b5e4841d92dcaebb4fa2acf454074eeb2c571517ac3671cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae18940ab920c723e970d89fde606b552e5b39f5fa33535cb6c7be09b6cff763`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 08 Dec 2023 19:55:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/welcome/index.html"
# Fri, 08 Dec 2023 19:55:16 GMT
ENV CADDY_VERSION=v2.7.6
# Fri, 08 Dec 2023 19:55:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b74311ec8263f30f6d36e5c8be151e8bc092b377789a55300d5671238b9043de5bd6db2bcefae32aa1e6fe94c47bbf02982c44a7871e5777b2596fdb20907cbf' ;; 		armhf)   binArch='armv6'; checksum='88756642ca412db3a8da7a40b518861a6f524a8ac704021e8451d3cb38746f24243b1e561f4eec07e1575200d06bfd098783d2b7ee7ee07a971aed1c677da6e6' ;; 		armv7)   binArch='armv7'; checksum='118776e879c280556abb7c03ff7c0081eda23c2aee0472aef176f733785e9501defaeaf334cd2443e31294809beafaea831d2e695aa68045160082aa3a966e2f' ;; 		aarch64) binArch='arm64'; checksum='62252ade5e8dcec13a66154ee1978d959370be049cce52e7c4edefff14ef70bbb21630e3735092719bc3c31214e89dff99e55970ff0adec8ac0a94c6415b059a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='65d27fe53f5e4fa79f3476f8902071c907aab74db1a2616342be3714d4252219fbb53b174ef588e20c51e7cfac84376c7a0a608091c2fe83b31dbf59dabeb237' ;; 		s390x)   binArch='s390x'; checksum='c562190962a2db0248a4190616dd2ebaa02df2cf62f1a2c71f9d9de18af2a297df8000a06a11e8d3929dfd64f0c081d1e61961687ca220007459f2dbd0be2c81' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.6/caddy_2.7.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 08 Dec 2023 19:55:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 08 Dec 2023 19:55:17 GMT
ENV XDG_DATA_HOME=/data
# Fri, 08 Dec 2023 19:55:17 GMT
LABEL org.opencontainers.image.version=v2.7.6
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 08 Dec 2023 19:55:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 08 Dec 2023 19:55:18 GMT
EXPOSE 80
# Fri, 08 Dec 2023 19:55:18 GMT
EXPOSE 443
# Fri, 08 Dec 2023 19:55:18 GMT
EXPOSE 443/udp
# Fri, 08 Dec 2023 19:55:18 GMT
EXPOSE 2019
# Fri, 08 Dec 2023 19:55:18 GMT
WORKDIR /srv
# Fri, 08 Dec 2023 19:55:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f87e6bdbafc6710a3ed7bfbb4bb134e8d93bea992ab895c653cac0779389396`  
		Last Modified: Fri, 08 Dec 2023 19:55:35 GMT  
		Size: 7.5 KB (7529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874486d3ac5891d4df17819e02e1cdd3775748effa24bc53645cd2db841a0837`  
		Last Modified: Fri, 08 Dec 2023 19:55:36 GMT  
		Size: 13.6 MB (13568967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:f8db25c8783258ee73a7ab061dbcb53f5229be2510ab4c72cbb6fe5292fdd1a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17818230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4782f6a3e2f343e87b335a56846d9ae67a4a5aded358a8501a4fb5a076e92cef`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 08 Dec 2023 19:57:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/cd39178d252a610fee6aa8465c787d9c780007a2/welcome/index.html"
# Fri, 08 Dec 2023 19:57:07 GMT
ENV CADDY_VERSION=v2.7.6
# Fri, 08 Dec 2023 19:57:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b74311ec8263f30f6d36e5c8be151e8bc092b377789a55300d5671238b9043de5bd6db2bcefae32aa1e6fe94c47bbf02982c44a7871e5777b2596fdb20907cbf' ;; 		armhf)   binArch='armv6'; checksum='88756642ca412db3a8da7a40b518861a6f524a8ac704021e8451d3cb38746f24243b1e561f4eec07e1575200d06bfd098783d2b7ee7ee07a971aed1c677da6e6' ;; 		armv7)   binArch='armv7'; checksum='118776e879c280556abb7c03ff7c0081eda23c2aee0472aef176f733785e9501defaeaf334cd2443e31294809beafaea831d2e695aa68045160082aa3a966e2f' ;; 		aarch64) binArch='arm64'; checksum='62252ade5e8dcec13a66154ee1978d959370be049cce52e7c4edefff14ef70bbb21630e3735092719bc3c31214e89dff99e55970ff0adec8ac0a94c6415b059a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='65d27fe53f5e4fa79f3476f8902071c907aab74db1a2616342be3714d4252219fbb53b174ef588e20c51e7cfac84376c7a0a608091c2fe83b31dbf59dabeb237' ;; 		s390x)   binArch='s390x'; checksum='c562190962a2db0248a4190616dd2ebaa02df2cf62f1a2c71f9d9de18af2a297df8000a06a11e8d3929dfd64f0c081d1e61961687ca220007459f2dbd0be2c81' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.6/caddy_2.7.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 08 Dec 2023 19:57:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 08 Dec 2023 19:57:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 08 Dec 2023 19:57:12 GMT
LABEL org.opencontainers.image.version=v2.7.6
# Fri, 08 Dec 2023 19:57:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 08 Dec 2023 19:57:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 08 Dec 2023 19:57:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 08 Dec 2023 19:57:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 08 Dec 2023 19:57:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 08 Dec 2023 19:57:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 08 Dec 2023 19:57:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 08 Dec 2023 19:57:13 GMT
EXPOSE 80
# Fri, 08 Dec 2023 19:57:13 GMT
EXPOSE 443
# Fri, 08 Dec 2023 19:57:14 GMT
EXPOSE 443/udp
# Fri, 08 Dec 2023 19:57:14 GMT
EXPOSE 2019
# Fri, 08 Dec 2023 19:57:14 GMT
WORKDIR /srv
# Fri, 08 Dec 2023 19:57:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa042ad4816c33e4f907bbf008abef2397efe2b3fc378430b2b925663a088370`  
		Last Modified: Fri, 08 Dec 2023 19:57:43 GMT  
		Size: 7.5 KB (7526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ceec9a3d819911fec4d039d31e2e3e38214fa45cb8384e8f047b5588724355`  
		Last Modified: Fri, 08 Dec 2023 19:57:45 GMT  
		Size: 14.2 MB (14238302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
