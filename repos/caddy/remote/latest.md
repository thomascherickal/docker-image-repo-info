## `caddy:latest`

```console
$ docker pull caddy@sha256:1d712564b81aa268e40bc2b46bd29c36730272500049bef3803925beb1dc60b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:e1bf58da88319a06e9f4f02694eec16ee18df200faf669572542f7c4ef0adf85
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15166028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114d8ea32dd6038d8a77e6ae85dcef22c856c39ebb2ff4b4300819747ce1c7ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Fri, 24 Apr 2020 13:39:05 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Fri, 24 Apr 2020 13:39:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 24 Apr 2020 13:39:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 24 Apr 2020 13:39:07 GMT
ENV XDG_DATA_HOME=/data
# Fri, 24 Apr 2020 13:39:08 GMT
VOLUME [/config]
# Fri, 24 Apr 2020 13:39:08 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 13:39:08 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Fri, 24 Apr 2020 13:39:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 24 Apr 2020 13:39:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 24 Apr 2020 13:39:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 24 Apr 2020 13:39:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 24 Apr 2020 13:39:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 24 Apr 2020 13:39:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 24 Apr 2020 13:39:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 24 Apr 2020 13:39:09 GMT
EXPOSE 80
# Fri, 24 Apr 2020 13:39:10 GMT
EXPOSE 443
# Fri, 24 Apr 2020 13:39:10 GMT
EXPOSE 2019
# Fri, 24 Apr 2020 13:39:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7649e2acac0467d46b2e43138e8175c21bed9157d57aeefc989aa81f0c96ccce`  
		Last Modified: Fri, 24 Apr 2020 13:39:24 GMT  
		Size: 12.0 MB (12028393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:573c522b9b615f0a170cb67d8b60eb04fbd6ec71f143e144491d8a0c437eced3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61c594384ee76fb98cb52dd996ca5fb8fb3bd1c1e0fea7d3779446991dc3b64a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Mon, 04 May 2020 18:49:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 May 2020 18:49:29 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 May 2020 18:49:30 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 May 2020 18:49:30 GMT
VOLUME [/config]
# Mon, 04 May 2020 18:49:31 GMT
VOLUME [/data]
# Mon, 04 May 2020 18:49:31 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Mon, 04 May 2020 18:49:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 May 2020 18:49:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 May 2020 18:49:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 May 2020 18:49:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 May 2020 18:49:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 May 2020 18:49:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 May 2020 18:49:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 May 2020 18:49:36 GMT
EXPOSE 80
# Mon, 04 May 2020 18:49:37 GMT
EXPOSE 443
# Mon, 04 May 2020 18:49:37 GMT
EXPOSE 2019
# Mon, 04 May 2020 18:49:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5426d82a800682232a3a79b956267dc1bbbe42a1824db86c051bd568dff0bc65`  
		Last Modified: Mon, 04 May 2020 18:51:13 GMT  
		Size: 11.4 MB (11445869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:de0598b774fa1273354856d3a911b6d5ac9977d500725d89926dd3fcb84a5970
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14189653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9427d09d1d14daafc58c13d3701f509defe538752a94e7a3d15fe4b3b595408`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 23 Apr 2020 23:23:05 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Thu, 23 Apr 2020 23:23:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 23 Apr 2020 23:23:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 23 Apr 2020 23:23:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 23 Apr 2020 23:23:22 GMT
VOLUME [/config]
# Thu, 23 Apr 2020 23:23:23 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 23:23:24 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Thu, 23 Apr 2020 23:23:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 23 Apr 2020 23:23:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 23 Apr 2020 23:23:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 23 Apr 2020 23:23:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 23 Apr 2020 23:23:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 23 Apr 2020 23:23:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 23 Apr 2020 23:23:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 23 Apr 2020 23:23:31 GMT
EXPOSE 80
# Thu, 23 Apr 2020 23:23:32 GMT
EXPOSE 443
# Thu, 23 Apr 2020 23:23:33 GMT
EXPOSE 2019
# Thu, 23 Apr 2020 23:23:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c40522962f3fe09cd98fd4eaa89dd882a4696b160f7107066ec610a424d2b5`  
		Last Modified: Thu, 23 Apr 2020 23:23:55 GMT  
		Size: 11.4 MB (11443876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bd3d569cc384e9a4325347210ee73b8315cecb9b520745e85482c900d22f4246
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7688159d39640bfa4b93c57af764aa2610560d795d63f5abd63d95a9916fff4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Mon, 04 May 2020 18:39:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 May 2020 18:39:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 May 2020 18:39:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 May 2020 18:39:48 GMT
VOLUME [/config]
# Mon, 04 May 2020 18:39:49 GMT
VOLUME [/data]
# Mon, 04 May 2020 18:39:51 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Mon, 04 May 2020 18:39:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 May 2020 18:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 May 2020 18:39:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 May 2020 18:39:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 May 2020 18:39:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 May 2020 18:40:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 May 2020 18:40:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 May 2020 18:40:02 GMT
EXPOSE 80
# Mon, 04 May 2020 18:40:04 GMT
EXPOSE 443
# Mon, 04 May 2020 18:40:05 GMT
EXPOSE 2019
# Mon, 04 May 2020 18:40:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2097dd602dad0efc9190dcd5d925993db58b65835f57bd151fa8d6160ac16e`  
		Last Modified: Mon, 04 May 2020 18:41:22 GMT  
		Size: 11.0 MB (11049972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1158; amd64

```console
$ docker pull caddy@sha256:2ab18a688a17a73c73047e5ee0791b1594a830ece6b74014e0c19dd1434a1ed2
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2288047988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93a2c9ae0176adbe355c01d72309af92c7283f84bb324671811158d2fee279c2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 23:15:34 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Mon, 20 Apr 2020 23:35:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 20 Apr 2020 23:35:07 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:26:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('482652dbe7600d4d324c837a00eddf58254aeff57315afa1547fc61daefcb2f8952df8f3f8ec9c44e9ec919d1bfc908aeabe68b7d780d988d68e78581202d7ca')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 21 Apr 2020 00:26:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 21 Apr 2020 00:26:26 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 21 Apr 2020 00:26:27 GMT
VOLUME [c:/config]
# Tue, 21 Apr 2020 00:26:27 GMT
VOLUME [c:/data]
# Tue, 21 Apr 2020 00:26:28 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:26:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:26:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:26:31 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:26:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:26:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:26:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:26:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:26:36 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:26:37 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:26:37 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:26:54 GMT
RUN caddy version
# Tue, 21 Apr 2020 00:26:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9153fe178f6c24d737a32e64b5339d6c98c6f3510991a022194840e79bc4db4f`  
		Last Modified: Mon, 20 Apr 2020 23:21:13 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0181e8dc490f55c1e3f46913e0869af835174a08254258ad3e4927a8337d162`  
		Last Modified: Tue, 21 Apr 2020 00:27:35 GMT  
		Size: 4.7 MB (4701412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971ceadc9a2d2d0519526f38479ebb0ef5d33b92a0c5d39414b1649e4fba38e`  
		Last Modified: Tue, 21 Apr 2020 00:27:34 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9065a038cb7734374fcea435c47e0de04609a6f32be2e32c9d8248bf78166d6`  
		Last Modified: Tue, 21 Apr 2020 00:27:35 GMT  
		Size: 12.3 MB (12311819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c903d00aadf71c5c2dc3e31bdac91b87f5ef686dd6965a113e0628237eafe315`  
		Last Modified: Tue, 21 Apr 2020 00:27:31 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc84ffd4699c74078fff05c3e730793db7b218ba3235e982e1707fee66346b0`  
		Last Modified: Tue, 21 Apr 2020 00:27:31 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7840ec68916babca48fcfb77db033eddca77348cb742ba35119c1b1ef18491d1`  
		Last Modified: Tue, 21 Apr 2020 00:27:31 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d6542d3f2576dc2828c93b4acbbfd20a2f74b24ca222edf4124060bf88b6f7`  
		Last Modified: Tue, 21 Apr 2020 00:27:29 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f517507abfc2f4c42c0fb50dd9ba3e54d8aaa73f0da5bbb121bb38ae2d887b`  
		Last Modified: Tue, 21 Apr 2020 00:27:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8dafeec8f9d0a69ef2946a65d81ffae4df619b3286fa392add7d85ef898f37`  
		Last Modified: Tue, 21 Apr 2020 00:27:28 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e80dfc60703b374d09f4590742f8cf993fc0644182bbeaa4296b5ea3b36c14`  
		Last Modified: Tue, 21 Apr 2020 00:27:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c72b00f45cd8aa241caf326ac01c2634d62c9fabd5fb358d3671c980dacc2c`  
		Last Modified: Tue, 21 Apr 2020 00:27:26 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25526e8a896c4626208a748cae4029fe1613c47f28ad3f9e9d55450f5916c1ee`  
		Last Modified: Tue, 21 Apr 2020 00:27:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c974c0e14501eee29d001187318bdeefc1aaba598c845506f6525724f5ac`  
		Last Modified: Tue, 21 Apr 2020 00:27:26 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1756820635d22e919aa8f5da472c81619db165749f3b086685d532a349fff02`  
		Last Modified: Tue, 21 Apr 2020 00:27:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a608957249e89c39935e4a8e2fb0af12852ef3b3840ea10c4cb30fc6039ed61c`  
		Last Modified: Tue, 21 Apr 2020 00:27:26 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85245104d1e11ca59b44fd743be5d1a4f28babcda09ef1aea690b6db266786d0`  
		Last Modified: Tue, 21 Apr 2020 00:27:23 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2643b850e92d7157bc1d3db1c1edd8b2fde7bbce2930929fd9b69a8cc9a02670`  
		Last Modified: Tue, 21 Apr 2020 00:27:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f870e9d8082cafffb8f271cc4bc83db3849f7ee8c237eb536a91bbe188bede`  
		Last Modified: Tue, 21 Apr 2020 00:27:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0e70a530470c9e404c4046eda7e1988375bae1b3fefef1f24733652d0ce4be`  
		Last Modified: Tue, 21 Apr 2020 00:27:24 GMT  
		Size: 305.8 KB (305815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afed809a03adfaac23b3f609288bc4f6249cdbba3f7bea1e502ff7fc34baaa10`  
		Last Modified: Tue, 21 Apr 2020 00:27:23 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3630; amd64

```console
$ docker pull caddy@sha256:ce36943bd1dd39de8f8d6b47eaab078dc2b47a5a3c4ce7e065d18b7cd672e911
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751106345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5fbf7d2d002a25cee5fcc7ac5259a43b287f575e9627946e2582f27295387a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 23:17:30 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Mon, 20 Apr 2020 23:35:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 20 Apr 2020 23:35:30 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Mon, 20 Apr 2020 23:49:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('482652dbe7600d4d324c837a00eddf58254aeff57315afa1547fc61daefcb2f8952df8f3f8ec9c44e9ec919d1bfc908aeabe68b7d780d988d68e78581202d7ca')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 20 Apr 2020 23:49:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 20 Apr 2020 23:49:36 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 20 Apr 2020 23:49:37 GMT
VOLUME [c:/config]
# Mon, 20 Apr 2020 23:49:39 GMT
VOLUME [c:/data]
# Mon, 20 Apr 2020 23:49:39 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Mon, 20 Apr 2020 23:49:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 20 Apr 2020 23:49:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 20 Apr 2020 23:49:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 20 Apr 2020 23:49:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 20 Apr 2020 23:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 20 Apr 2020 23:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 20 Apr 2020 23:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 20 Apr 2020 23:49:47 GMT
EXPOSE 80
# Mon, 20 Apr 2020 23:49:48 GMT
EXPOSE 443
# Mon, 20 Apr 2020 23:49:49 GMT
EXPOSE 2019
# Mon, 20 Apr 2020 23:50:29 GMT
RUN caddy version
# Mon, 20 Apr 2020 23:50:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72ac64d06edc38376c754491fd7ced4aa035af4e675cdc3ac928ea71101af9d`  
		Last Modified: Tue, 21 Apr 2020 00:27:58 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d9ac51d67cd523925abe19d1fefd0f5e5de96dd7f4210eebd601cd07940879`  
		Last Modified: Tue, 21 Apr 2020 00:27:59 GMT  
		Size: 5.4 MB (5407793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efd1ee2ff7bdfd99171e6f519ce15fec5cae88d015c7fe68f90bc0a06c6d931`  
		Last Modified: Tue, 21 Apr 2020 00:27:55 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6a8fefdc6e0c56bb106524f505c0946830f2f05160508c322fe12c577ff6c3`  
		Last Modified: Tue, 21 Apr 2020 00:28:00 GMT  
		Size: 17.3 MB (17345135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109a9eb27291be9eca6eba7e86637f2e89299d52c9b7e6e8732d3142413a0cdd`  
		Last Modified: Tue, 21 Apr 2020 00:27:54 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbda073322d4050091a4128fbee7a86f3a44a20a5e48a9a757b75f947e55389f`  
		Last Modified: Tue, 21 Apr 2020 00:27:54 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25bd862ac7d8a4e4dd071336125b456299f48e50a0521b24c85d960076e0199`  
		Last Modified: Tue, 21 Apr 2020 00:27:54 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1f91e729270af491f0aa53bb55300e2d82a22aad5c79d552884f60da6cd4e4`  
		Last Modified: Tue, 21 Apr 2020 00:27:53 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad733b24685a79f25a39ff32f4aa315ebfae9df99740c7432be70bad755dae2`  
		Last Modified: Tue, 21 Apr 2020 00:27:52 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57efa182f8d96025abbeabbf9263c42537fda0ad5a4f59a312d5ece4cfcd508`  
		Last Modified: Tue, 21 Apr 2020 00:27:52 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b347e572e899a9b99fd7aaf5f29345aaf65ce32e7a121771c8021c662a1f4f`  
		Last Modified: Tue, 21 Apr 2020 00:27:52 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9eb61d24eaffc90b7870772f420233e1520893a9ad25c44bb055f787ee2705`  
		Last Modified: Tue, 21 Apr 2020 00:27:50 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8150597f5e499c8bd034ca80229afd4aa88471b8efe5443772e1e92fd066b751`  
		Last Modified: Tue, 21 Apr 2020 00:27:50 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61038c548fa7ceffb45bf18cb81982dc221149295379caa793056c88590d860f`  
		Last Modified: Tue, 21 Apr 2020 00:27:49 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5e285cc3c3c7d19ff1a8aba39a5fa042cb718bae816d46b3a59358f47378ee`  
		Last Modified: Tue, 21 Apr 2020 00:27:50 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a118b6f4d69c1f8b687dd9af977ee2f24bc5941ca9b8cc69ad80e487f9fa283b`  
		Last Modified: Tue, 21 Apr 2020 00:27:49 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639f711254bc6fec0693a5e59eec876b3e388671ebee36fb7ff665c7f840da97`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97944dcb26ce67036f0a5d96e3a9d8b4911945df4e4506284becb7d72aacca1`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049d194f6bb19cb62503770c5b949a2d2806848f6dd8c2c0fa755818a8741f`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c13083a16372e822e86a1958ba180d6ad32f22d0d13ca941a74351a7d531a18`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 265.2 KB (265183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8883ec4854456b8d05c3ba46b3e7c7eec6e91ad0d596e374178fc795cda12a13`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
