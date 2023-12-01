## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:9821d1ef822957bf0ac22f9c6e26ad6a3198604f29b3b79194acba7ccaff4532
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

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
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
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

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

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
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
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

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

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
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
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
