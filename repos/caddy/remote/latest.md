## `caddy:latest`

```console
$ docker pull caddy@sha256:2ec7f74a5fba05aca168edf9bd37ad27621d2ec5385a8d2bf0d1d4ce849e4f69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:af6a86c2b2f6444d9e823f01b606b0ea37be04d8a3313056874ba5c81c8bdffe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27077359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feec2b87e8a45f3ad435885c2c69158be1c7fbcad6405be61355e00d76113e9d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Apr 2020 23:43:04 GMT
RUN apk add --no-cache ca-certificates
# Mon, 13 Apr 2020 23:43:04 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 13 Apr 2020 23:43:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 14 Apr 2020 19:06:36 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 14 Apr 2020 19:06:36 GMT
ENV XDG_DATA_HOME=/data
# Tue, 14 Apr 2020 19:06:36 GMT
VOLUME [/config]
# Tue, 14 Apr 2020 19:06:37 GMT
VOLUME [/data]
# Tue, 14 Apr 2020 19:06:37 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:06:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 14 Apr 2020 19:06:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 14 Apr 2020 19:06:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 14 Apr 2020 19:06:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 14 Apr 2020 19:06:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 14 Apr 2020 19:06:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 14 Apr 2020 19:06:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 14 Apr 2020 19:06:38 GMT
EXPOSE 80
# Tue, 14 Apr 2020 19:06:38 GMT
EXPOSE 443
# Tue, 14 Apr 2020 19:06:38 GMT
EXPOSE 2019
# Tue, 14 Apr 2020 19:06:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34768c0e097ae8d61b298bc7f4f92fb388c048edba171f5b0ce6b43529fe44c`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 301.3 KB (301287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8542e370608b22a8c405d41ba15bb6318bb044928e806a24084eb77593ecac`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44085fbaaf595a39762cf4b2c622400a5b6fecc0339a1151cf0957c2b923fe06`  
		Last Modified: Tue, 14 Apr 2020 19:06:57 GMT  
		Size: 24.0 MB (23967050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:80026b4075882fc016416caa0783b19c1b1ac4ed49cda336765245eee0b1d5f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25818293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b87b98e19c001ce4d534704c2bcb3e81d67b07de4dca1641099ac130d019e53d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 14 Apr 2020 19:01:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 14 Apr 2020 19:01:23 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Tue, 14 Apr 2020 19:01:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Tue, 14 Apr 2020 19:01:27 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 14 Apr 2020 19:01:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 14 Apr 2020 19:01:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 14 Apr 2020 19:01:37 GMT
VOLUME [/config]
# Tue, 14 Apr 2020 19:01:40 GMT
VOLUME [/data]
# Tue, 14 Apr 2020 19:01:42 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 14 Apr 2020 19:01:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 14 Apr 2020 19:01:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 14 Apr 2020 19:01:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 14 Apr 2020 19:01:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 14 Apr 2020 19:01:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 14 Apr 2020 19:01:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 14 Apr 2020 19:01:54 GMT
EXPOSE 80
# Tue, 14 Apr 2020 19:01:56 GMT
EXPOSE 443
# Tue, 14 Apr 2020 19:01:57 GMT
EXPOSE 2019
# Tue, 14 Apr 2020 19:01:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5d46f4b0c463211700eecfa1fb5aea107eebee8f0954bb52e97c55374269d2`  
		Last Modified: Tue, 14 Apr 2020 19:03:54 GMT  
		Size: 301.6 KB (301624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3debeaf9ccc0de7352984299a94e2fe159d2da5ebe4cf4620e26bafc15272151`  
		Last Modified: Tue, 14 Apr 2020 19:03:54 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ea7abba3a6454366ff41ba6138e9c3365432b55b71ceddbc60b1f5330c8d7d`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 22.9 MB (22892243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d57b8c3f2bfa2f4d02421240113c93aeef5488e2ba05c6614dd974d6097fa3f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25572692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64e0a96e63271ccce1a2960cb7fe3244b0d1eac67fdcafceadb4b09b35fd2a9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Tue, 14 Apr 2020 19:01:22 GMT
RUN apk add --no-cache ca-certificates
# Tue, 14 Apr 2020 19:01:23 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Tue, 14 Apr 2020 19:01:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Tue, 14 Apr 2020 19:01:27 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 14 Apr 2020 19:01:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 14 Apr 2020 19:01:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 14 Apr 2020 19:01:37 GMT
VOLUME [/config]
# Tue, 14 Apr 2020 19:01:40 GMT
VOLUME [/data]
# Tue, 14 Apr 2020 19:01:42 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:01:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 14 Apr 2020 19:01:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 14 Apr 2020 19:01:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 14 Apr 2020 19:01:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 14 Apr 2020 19:01:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 14 Apr 2020 19:01:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 14 Apr 2020 19:01:54 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 14 Apr 2020 19:01:55 GMT
EXPOSE 80
# Tue, 14 Apr 2020 19:01:57 GMT
EXPOSE 443
# Tue, 14 Apr 2020 19:01:58 GMT
EXPOSE 2019
# Tue, 14 Apr 2020 19:01:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc78d383e9699647bdba17a1596a028860488035d0acd1b568dd08deb266fca7`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 300.6 KB (300604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e8f9ac40210e9852b63895bf8fcaec719afc0d457d820764f840923e946d15`  
		Last Modified: Tue, 14 Apr 2020 19:03:56 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd7a35cc439b98a9002c797a6d696033509111cbdd336152a4035731fb9875a`  
		Last Modified: Tue, 14 Apr 2020 19:04:02 GMT  
		Size: 22.8 MB (22845750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ffc93391ac36adf0d99b25d938d029ca8391faee55578f5d2fd849b7d871c98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25092628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3371571a058dd820a061840c1e5f15e0ef5c963a586c28e611a5b03e31b6c38d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 14 Apr 2020 19:01:20 GMT
RUN apk add --no-cache ca-certificates
# Tue, 14 Apr 2020 19:01:22 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Tue, 14 Apr 2020 19:01:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Tue, 14 Apr 2020 19:01:25 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:01:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 14 Apr 2020 19:01:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 14 Apr 2020 19:01:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 14 Apr 2020 19:01:33 GMT
VOLUME [/config]
# Tue, 14 Apr 2020 19:01:35 GMT
VOLUME [/data]
# Tue, 14 Apr 2020 19:01:36 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:01:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 14 Apr 2020 19:01:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 14 Apr 2020 19:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 14 Apr 2020 19:01:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 14 Apr 2020 19:01:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 14 Apr 2020 19:01:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 14 Apr 2020 19:01:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 14 Apr 2020 19:01:51 GMT
EXPOSE 80
# Tue, 14 Apr 2020 19:01:53 GMT
EXPOSE 443
# Tue, 14 Apr 2020 19:01:54 GMT
EXPOSE 2019
# Tue, 14 Apr 2020 19:01:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75f8cb084cea530c1f7c1a560af77329b9a47b765acef276eb64c7f39fb3e8f`  
		Last Modified: Tue, 14 Apr 2020 19:03:44 GMT  
		Size: 301.8 KB (301782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4f0757169a4c9a3174592d530b89006d7afca436c02ab2b3175f45a8c382b8`  
		Last Modified: Tue, 14 Apr 2020 19:03:45 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267e66a05fb3770e4ee6f1a6973eb597ce56083d3ef04b8334530b1a7f576c7`  
		Last Modified: Tue, 14 Apr 2020 19:03:49 GMT  
		Size: 22.1 MB (22061861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
