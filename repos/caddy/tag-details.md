<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2.0.0-rc.3`](#caddy200-rc3)
-	[`caddy:2.0.0-rc.3-alpine`](#caddy200-rc3-alpine)
-	[`caddy:2.0.0-rc.3-builder`](#caddy200-rc3-builder)
-	[`caddy:2.0.0-rc.3-windowsservercore`](#caddy200-rc3-windowsservercore)
-	[`caddy:2.0.0-rc.3-windowsservercore-1809`](#caddy200-rc3-windowsservercore-1809)
-	[`caddy:2.0.0-rc.3-windowsservercore-ltsc2016`](#caddy200-rc3-windowsservercore-ltsc2016)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2016`](#caddywindowsservercore-ltsc2016)

## `caddy:2.0.0-rc.3`

```console
$ docker pull caddy@sha256:f2f734c7a8369ac0b1ffdb284f52db7b28812712357185beec2c308730fc4d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `caddy:2.0.0-rc.3` - linux; amd64

```console
$ docker pull caddy@sha256:30abbbfe8151fa239f51cf9cb5ed51c705e7b016591de1a5cba1cbe596dd2ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15155960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9477d0c347fd32b124a4d4dc0c3270d2453f7b118b3d607731e3f220da3f05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:19:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:19:25 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:19:27 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:20 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c895336717654d7bf50758d2fe590a60610eb7d7168d12c6b6bb9887bae481d`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 318.6 KB (318556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e769246751713852fe7f4107628f489ad3068e3ef3d9180d8f282591fce3ae2`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 5.8 KB (5764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555f6fbb196736d103501b827439a43d1a6cba20ebff7df44f228f1798eb4ee`  
		Last Modified: Tue, 21 Apr 2020 00:24:36 GMT  
		Size: 12.0 MB (12028385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7ed08e071a11d38b7be1d9b2d68d6d15786980e2e6e1ee063e89493eb898a1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14409137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7460066cc8bd6b931cb96fcc0c855c2673b7923e5084718508000e664d50df61`
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
# Thu, 23 Apr 2020 17:42:34 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 23 Apr 2020 17:42:40 GMT
VOLUME [/config]
# Thu, 23 Apr 2020 17:42:41 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:42:41 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 23 Apr 2020 17:42:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 23 Apr 2020 17:42:46 GMT
EXPOSE 80
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 443
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 2019
# Thu, 23 Apr 2020 17:42:48 GMT
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
	-	`sha256:06e7b1f9bee864c12dd2ceef4062aa39220c9921e53de9328e46201a9706536f`  
		Last Modified: Thu, 23 Apr 2020 17:43:11 GMT  
		Size: 11.5 MB (11464427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3` - linux; arm variant v7

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

### `caddy:2.0.0-rc.3` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b4580ebabc4eed91b683f0980d117998aca158f6690e0e8f5e09771d48aa2fbf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14115062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659da137a1ca66bfa07139e8c1504fbdf9c0915f071736c4c42fa0fc091eeb63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:39:33 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:39:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:39:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:39:36 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:35 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:36 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:37 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:49 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:51 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:52 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8769f63ec8b31f05ebb26b0a58d55301ef35d1449a5f401e24fbd8fc966bfd21`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 319.1 KB (319126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaac47c6de0ab38444a53999b472ae63772dbb66155e37fc5014ee3f99d596e`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8eecc840bde75e030ca92b955c6466f7017e33fa7a48c96d5abb6b1473e778`  
		Last Modified: Tue, 21 Apr 2020 00:25:16 GMT  
		Size: 11.1 MB (11066952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3` - windows version 10.0.17763.1158; amd64

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

### `caddy:2.0.0-rc.3` - windows version 10.0.14393.3630; amd64

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

## `caddy:2.0.0-rc.3-alpine`

```console
$ docker pull caddy@sha256:c2e9e0c984a407aa5ca3e27e61fd7068f28a83da7ae84c0557583bafa471c31f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `caddy:2.0.0-rc.3-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:30abbbfe8151fa239f51cf9cb5ed51c705e7b016591de1a5cba1cbe596dd2ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15155960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9477d0c347fd32b124a4d4dc0c3270d2453f7b118b3d607731e3f220da3f05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:19:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:19:25 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:19:27 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:20 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c895336717654d7bf50758d2fe590a60610eb7d7168d12c6b6bb9887bae481d`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 318.6 KB (318556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e769246751713852fe7f4107628f489ad3068e3ef3d9180d8f282591fce3ae2`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 5.8 KB (5764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555f6fbb196736d103501b827439a43d1a6cba20ebff7df44f228f1798eb4ee`  
		Last Modified: Tue, 21 Apr 2020 00:24:36 GMT  
		Size: 12.0 MB (12028385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7ed08e071a11d38b7be1d9b2d68d6d15786980e2e6e1ee063e89493eb898a1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14409137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7460066cc8bd6b931cb96fcc0c855c2673b7923e5084718508000e664d50df61`
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
# Thu, 23 Apr 2020 17:42:34 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 23 Apr 2020 17:42:40 GMT
VOLUME [/config]
# Thu, 23 Apr 2020 17:42:41 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:42:41 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 23 Apr 2020 17:42:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 23 Apr 2020 17:42:46 GMT
EXPOSE 80
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 443
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 2019
# Thu, 23 Apr 2020 17:42:48 GMT
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
	-	`sha256:06e7b1f9bee864c12dd2ceef4062aa39220c9921e53de9328e46201a9706536f`  
		Last Modified: Thu, 23 Apr 2020 17:43:11 GMT  
		Size: 11.5 MB (11464427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3-alpine` - linux; arm variant v7

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

### `caddy:2.0.0-rc.3-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b4580ebabc4eed91b683f0980d117998aca158f6690e0e8f5e09771d48aa2fbf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14115062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659da137a1ca66bfa07139e8c1504fbdf9c0915f071736c4c42fa0fc091eeb63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:39:33 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:39:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:39:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:39:36 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:35 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:36 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:37 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:49 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:51 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:52 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8769f63ec8b31f05ebb26b0a58d55301ef35d1449a5f401e24fbd8fc966bfd21`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 319.1 KB (319126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaac47c6de0ab38444a53999b472ae63772dbb66155e37fc5014ee3f99d596e`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8eecc840bde75e030ca92b955c6466f7017e33fa7a48c96d5abb6b1473e778`  
		Last Modified: Tue, 21 Apr 2020 00:25:16 GMT  
		Size: 11.1 MB (11066952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-rc.3-builder`

```console
$ docker pull caddy@sha256:58dfd4e3cbef7b0b1048ef1f8713058b456434f0b5b0af49ace170a00bca62b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `caddy:2.0.0-rc.3-builder` - linux; amd64

```console
$ docker pull caddy@sha256:486d86fe70265203228afb9b9e6e7934019090c6686da9a9fb98579931a05778
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322863984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd06ca5bdeb1a36375ba63a93a06401045ebb7a6154830e973a6de5949242b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:02:02 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:06:10 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:11:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:11:13 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:11:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:11:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:11:16 GMT
WORKDIR /go
# Mon, 13 Apr 2020 23:43:21 GMT
WORKDIR /src
# Mon, 13 Apr 2020 23:43:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 13 Apr 2020 23:43:24 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:27 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 13 Apr 2020 23:43:27 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 13 Apr 2020 23:43:57 GMT
RUN go get -d ./...
# Mon, 13 Apr 2020 23:43:59 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 13 Apr 2020 23:43:59 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c732a2540651eb09faab95b03b3b5928ab23e096fae0006bdc2abf9e0cb5bfb4`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 301.3 KB (301283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2225181d6bcfb7877529a7257ff207cb14e52831420f770cbc2187031b6228`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdfa13e5b48c976ba308826b27a4978c2ffe6833efcfcfc0bd40dbf25e88455`  
		Last Modified: Wed, 08 Apr 2020 23:26:23 GMT  
		Size: 132.0 MB (132012220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c48a539365d2d572e18de4a42ab11b02d9870a17bf1f65160d7fcbbd0423263`  
		Last Modified: Wed, 08 Apr 2020 23:25:47 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947fdad36c6d1e2fd7b618aa1a49dfabaa1ff9d6fb85a195e2437c2b9ac78142`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199e6b2236a218d72efd03fc1fa0971c00c87439722e1a40269b7edfd910b79`  
		Last Modified: Mon, 13 Apr 2020 23:44:28 GMT  
		Size: 8.2 MB (8155831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732862f7439776bbe7cc313ed1e10454506f168429234c0daea17d6c48a9692`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 2.7 MB (2744273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54fb1573600e831b250c83cb9dc699bab8aa12040568d9ee542fb8d09c1d99`  
		Last Modified: Mon, 13 Apr 2020 23:45:02 GMT  
		Size: 176.8 MB (176846093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e336ec02e20348f57d1ef8151ecfcd216777f5489f01b29164883ec496bcbb`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6f8a2da1c847ae8cd10d1f3e37ad75cc0ba17c5e9b4f7e68fdd3b7cffb5482`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c9e71494cec26fe243c54231ae6fe4612a24fba7642b2782a2003bd4ac925f77
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318301249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b7f3bccf28346106c5d13d871e3b568057fec490d1f94bb04447e57ff90fd2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:43:45 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 17:49:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 17:49:50 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 17:49:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 17:49:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 17:49:53 GMT
WORKDIR /go
# Fri, 24 Apr 2020 00:01:08 GMT
WORKDIR /src
# Fri, 24 Apr 2020 00:01:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 24 Apr 2020 00:01:22 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Fri, 24 Apr 2020 00:01:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 24 Apr 2020 00:01:52 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 24 Apr 2020 00:04:31 GMT
RUN go get -d ./...
# Fri, 24 Apr 2020 00:04:38 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Fri, 24 Apr 2020 00:04:46 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851f1e9e77f7c701487b8ba5a7a0c915267b412d298572641c41785cacdb0a87`  
		Last Modified: Thu, 23 Apr 2020 18:04:01 GMT  
		Size: 128.1 MB (128149566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8512d94a71aa9475406b77a5df2ea5a15483204ab412358643fbe90c4af6c63`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515fa8cb76d9c64fedf8066a5d83b006a3f31d3f77bb6fda67c2e36668c18ab`  
		Last Modified: Fri, 24 Apr 2020 00:05:13 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14562a711f9706a0fb683480cf3849913e6b3f11d3599c62e4d1f9e831a46bf5`  
		Last Modified: Fri, 24 Apr 2020 00:05:12 GMT  
		Size: 7.8 MB (7794673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b172f9b87cc50b54dd1b3ec4a0a0d2e28b44b924e8f0602b2ba7a1a93987237d`  
		Last Modified: Fri, 24 Apr 2020 00:05:10 GMT  
		Size: 2.6 MB (2583752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbdcf6d6318b0e66c309c8d344563f2c4c5fada8a8764f7b513dbecd956170`  
		Last Modified: Fri, 24 Apr 2020 00:06:03 GMT  
		Size: 176.9 MB (176850568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35003bc5bd2fabea9a8e09f2761c662d1ce95e5d3e829a07ea2b619b5e35e6`  
		Last Modified: Fri, 24 Apr 2020 00:05:11 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ba293916f1b61d0eee5c397f11e2e206ffaa0c54d17f2bfb328da7e6f09743`  
		Last Modified: Fri, 24 Apr 2020 00:05:10 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c6b2f1f5d52cfbabf244af757effe7b6ddc142acdb15ef5d8dc7452a9659b795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.9 MB (316942094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516ec248376a670b87153cbe61efb69b30615826ae2ec1ee48034a951a771e92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:47:15 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:47:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:11:43 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:14:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:14:23 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:14:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:14:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:14:31 GMT
WORKDIR /go
# Tue, 14 Apr 2020 19:02:05 GMT
WORKDIR /src
# Tue, 14 Apr 2020 19:02:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 14 Apr 2020 19:02:10 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:02:15 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 14 Apr 2020 19:02:17 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 14 Apr 2020 19:03:31 GMT
RUN go get -d ./...
# Tue, 14 Apr 2020 19:03:39 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 14 Apr 2020 19:03:41 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c66f8509bb56e1ead748baf3433dcad3c1fa170146d5d7d06506b9a80f367`  
		Last Modified: Mon, 23 Mar 2020 23:53:18 GMT  
		Size: 300.6 KB (300602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf5f16b98b20e6e4f07e24e93de1018e88310a49963dc147c370d360a02fdbb`  
		Last Modified: Mon, 23 Mar 2020 23:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a38fd97575c34aedd91676d7643f6dbf66a1bca83f7d010e631807b96dae74`  
		Last Modified: Wed, 08 Apr 2020 23:25:03 GMT  
		Size: 127.8 MB (127774109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61bd435de55167e1a5a8cbdd73838375b819c98df2c23be5991140c00cbfd9a`  
		Last Modified: Wed, 08 Apr 2020 23:24:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a743cd83ba00508dd353a743708e6e434e2f56a1abdc6f2156d953839d646a1`  
		Last Modified: Tue, 14 Apr 2020 19:04:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928c849f33d759a505e159745da8960d19460b8735d7a08631ee817549c57d5`  
		Last Modified: Tue, 14 Apr 2020 19:04:11 GMT  
		Size: 7.0 MB (7010480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe4dbb3884a7fa0c551818da659e9c4d3f97f13eb6d53634655e97f9bd2f0d`  
		Last Modified: Tue, 14 Apr 2020 19:04:10 GMT  
		Size: 2.6 MB (2584042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb4bc7d74da5ae926bd30beea4c4abe59b6c0bb76705fb4f6b83391b591ecd7`  
		Last Modified: Tue, 14 Apr 2020 19:04:53 GMT  
		Size: 176.9 MB (176851243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fb3f4c0251d63ed371fb8a24333c2d9f9dada8830bad6af323550a4276f828`  
		Last Modified: Tue, 14 Apr 2020 19:04:09 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcea70e4e7db2fed8fb230f66d27fc46446054a0cdc6f6a342235480e7a248`  
		Last Modified: Tue, 14 Apr 2020 19:04:07 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-rc.3-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:75a990032363651bf7b39167b9e44e70cb8e6d4ae814545a2274a74005ce8660
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317221628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb140d2ac2499d88e26b91f2219f57edca78ae1597261d9799cb9519bf9f2e24`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:58:12 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 22:58:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:11:00 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:13:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:13:19 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:13:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:13:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:13:22 GMT
WORKDIR /go
# Tue, 14 Apr 2020 19:02:03 GMT
WORKDIR /src
# Tue, 14 Apr 2020 19:02:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 14 Apr 2020 19:02:08 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:02:12 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 14 Apr 2020 19:02:13 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 14 Apr 2020 19:03:13 GMT
RUN go get -d ./...
# Tue, 14 Apr 2020 19:03:15 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 14 Apr 2020 19:03:21 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d4106c43952870e20bfb808275012c22e6244af6eff1e916f446f7d338d0d`  
		Last Modified: Mon, 23 Mar 2020 23:03:34 GMT  
		Size: 301.8 KB (301778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f0a4e33d457336c22ac08eaec4609be330959ccdfefdb342be1045df4d26f0`  
		Last Modified: Mon, 23 Mar 2020 23:03:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44acbbdbf71f1d00fa6d0011bb10b82bef26b421a579bcf3a3491dced9f8233e`  
		Last Modified: Wed, 08 Apr 2020 23:21:31 GMT  
		Size: 126.4 MB (126405787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d054599df8f57e1578fdc2c554a9ac6124bf04f808dc623ef7f6548230fa3b5f`  
		Last Modified: Wed, 08 Apr 2020 23:20:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcee4e573bebbed33479e125fd8abf1f3debd0a7aee2137f55b67d9c38a79be`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968260b321a071a55eb891faac5f738bc2c3340a7843fc9ebd092902475f6fb3`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 8.4 MB (8353090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f7e47a5a4e440d1d8c40f1b42638e70ea0fbf9b5635f0145f58768993763d6`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 2.6 MB (2584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e682841e5eb376ed223cc26d628878cb76d53d943e6f205310f7294f212717`  
		Last Modified: Tue, 14 Apr 2020 19:04:33 GMT  
		Size: 176.9 MB (176852681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdb1a37f36e66ea176ba211db0396ddcf52e5c11bc8c335ad3814c1f091f33`  
		Last Modified: Tue, 14 Apr 2020 19:03:58 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d540e0414cc6a26d9aed38f141af756f0c60e88bb278d4807bda8d6b5939314`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-rc.3-windowsservercore`

```console
$ docker pull caddy@sha256:844b493cfdc844bf46ee328445e730513b81ca771a0b425f90381f2cd315102e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `caddy:2.0.0-rc.3-windowsservercore` - windows version 10.0.17763.1158; amd64

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

### `caddy:2.0.0-rc.3-windowsservercore` - windows version 10.0.14393.3630; amd64

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

## `caddy:2.0.0-rc.3-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9efbf07db38c66e53ee0497ba8229156e6ebc26a070d2fbddbdf6f6be715e5ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `caddy:2.0.0-rc.3-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

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

## `caddy:2.0.0-rc.3-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:540bc831c83dfe88a9d469750f2d8228fd14627e1cb6433a4e6b9470190c505e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `caddy:2.0.0-rc.3-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

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

## `caddy:alpine`

```console
$ docker pull caddy@sha256:c2e9e0c984a407aa5ca3e27e61fd7068f28a83da7ae84c0557583bafa471c31f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:30abbbfe8151fa239f51cf9cb5ed51c705e7b016591de1a5cba1cbe596dd2ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15155960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9477d0c347fd32b124a4d4dc0c3270d2453f7b118b3d607731e3f220da3f05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:19:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:19:25 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:19:27 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:20 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c895336717654d7bf50758d2fe590a60610eb7d7168d12c6b6bb9887bae481d`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 318.6 KB (318556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e769246751713852fe7f4107628f489ad3068e3ef3d9180d8f282591fce3ae2`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 5.8 KB (5764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555f6fbb196736d103501b827439a43d1a6cba20ebff7df44f228f1798eb4ee`  
		Last Modified: Tue, 21 Apr 2020 00:24:36 GMT  
		Size: 12.0 MB (12028385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7ed08e071a11d38b7be1d9b2d68d6d15786980e2e6e1ee063e89493eb898a1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14409137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7460066cc8bd6b931cb96fcc0c855c2673b7923e5084718508000e664d50df61`
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
# Thu, 23 Apr 2020 17:42:34 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 23 Apr 2020 17:42:40 GMT
VOLUME [/config]
# Thu, 23 Apr 2020 17:42:41 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:42:41 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 23 Apr 2020 17:42:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 23 Apr 2020 17:42:46 GMT
EXPOSE 80
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 443
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 2019
# Thu, 23 Apr 2020 17:42:48 GMT
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
	-	`sha256:06e7b1f9bee864c12dd2ceef4062aa39220c9921e53de9328e46201a9706536f`  
		Last Modified: Thu, 23 Apr 2020 17:43:11 GMT  
		Size: 11.5 MB (11464427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

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

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b4580ebabc4eed91b683f0980d117998aca158f6690e0e8f5e09771d48aa2fbf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14115062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659da137a1ca66bfa07139e8c1504fbdf9c0915f071736c4c42fa0fc091eeb63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:39:33 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:39:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:39:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:39:36 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:35 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:36 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:37 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:49 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:51 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:52 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8769f63ec8b31f05ebb26b0a58d55301ef35d1449a5f401e24fbd8fc966bfd21`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 319.1 KB (319126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaac47c6de0ab38444a53999b472ae63772dbb66155e37fc5014ee3f99d596e`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8eecc840bde75e030ca92b955c6466f7017e33fa7a48c96d5abb6b1473e778`  
		Last Modified: Tue, 21 Apr 2020 00:25:16 GMT  
		Size: 11.1 MB (11066952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:58dfd4e3cbef7b0b1048ef1f8713058b456434f0b5b0af49ace170a00bca62b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:486d86fe70265203228afb9b9e6e7934019090c6686da9a9fb98579931a05778
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322863984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd06ca5bdeb1a36375ba63a93a06401045ebb7a6154830e973a6de5949242b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:02:02 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:06:10 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:11:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:11:13 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:11:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:11:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:11:16 GMT
WORKDIR /go
# Mon, 13 Apr 2020 23:43:21 GMT
WORKDIR /src
# Mon, 13 Apr 2020 23:43:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 13 Apr 2020 23:43:24 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:27 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 13 Apr 2020 23:43:27 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 13 Apr 2020 23:43:57 GMT
RUN go get -d ./...
# Mon, 13 Apr 2020 23:43:59 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 13 Apr 2020 23:43:59 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c732a2540651eb09faab95b03b3b5928ab23e096fae0006bdc2abf9e0cb5bfb4`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 301.3 KB (301283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2225181d6bcfb7877529a7257ff207cb14e52831420f770cbc2187031b6228`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdfa13e5b48c976ba308826b27a4978c2ffe6833efcfcfc0bd40dbf25e88455`  
		Last Modified: Wed, 08 Apr 2020 23:26:23 GMT  
		Size: 132.0 MB (132012220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c48a539365d2d572e18de4a42ab11b02d9870a17bf1f65160d7fcbbd0423263`  
		Last Modified: Wed, 08 Apr 2020 23:25:47 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947fdad36c6d1e2fd7b618aa1a49dfabaa1ff9d6fb85a195e2437c2b9ac78142`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199e6b2236a218d72efd03fc1fa0971c00c87439722e1a40269b7edfd910b79`  
		Last Modified: Mon, 13 Apr 2020 23:44:28 GMT  
		Size: 8.2 MB (8155831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732862f7439776bbe7cc313ed1e10454506f168429234c0daea17d6c48a9692`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 2.7 MB (2744273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54fb1573600e831b250c83cb9dc699bab8aa12040568d9ee542fb8d09c1d99`  
		Last Modified: Mon, 13 Apr 2020 23:45:02 GMT  
		Size: 176.8 MB (176846093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e336ec02e20348f57d1ef8151ecfcd216777f5489f01b29164883ec496bcbb`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6f8a2da1c847ae8cd10d1f3e37ad75cc0ba17c5e9b4f7e68fdd3b7cffb5482`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c9e71494cec26fe243c54231ae6fe4612a24fba7642b2782a2003bd4ac925f77
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318301249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b7f3bccf28346106c5d13d871e3b568057fec490d1f94bb04447e57ff90fd2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Apr 2020 17:43:45 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 17:49:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 17:49:50 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 17:49:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 17:49:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 17:49:53 GMT
WORKDIR /go
# Fri, 24 Apr 2020 00:01:08 GMT
WORKDIR /src
# Fri, 24 Apr 2020 00:01:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 24 Apr 2020 00:01:22 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Fri, 24 Apr 2020 00:01:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 24 Apr 2020 00:01:52 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 24 Apr 2020 00:04:31 GMT
RUN go get -d ./...
# Fri, 24 Apr 2020 00:04:38 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Fri, 24 Apr 2020 00:04:46 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851f1e9e77f7c701487b8ba5a7a0c915267b412d298572641c41785cacdb0a87`  
		Last Modified: Thu, 23 Apr 2020 18:04:01 GMT  
		Size: 128.1 MB (128149566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8512d94a71aa9475406b77a5df2ea5a15483204ab412358643fbe90c4af6c63`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515fa8cb76d9c64fedf8066a5d83b006a3f31d3f77bb6fda67c2e36668c18ab`  
		Last Modified: Fri, 24 Apr 2020 00:05:13 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14562a711f9706a0fb683480cf3849913e6b3f11d3599c62e4d1f9e831a46bf5`  
		Last Modified: Fri, 24 Apr 2020 00:05:12 GMT  
		Size: 7.8 MB (7794673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b172f9b87cc50b54dd1b3ec4a0a0d2e28b44b924e8f0602b2ba7a1a93987237d`  
		Last Modified: Fri, 24 Apr 2020 00:05:10 GMT  
		Size: 2.6 MB (2583752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbdcf6d6318b0e66c309c8d344563f2c4c5fada8a8764f7b513dbecd956170`  
		Last Modified: Fri, 24 Apr 2020 00:06:03 GMT  
		Size: 176.9 MB (176850568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35003bc5bd2fabea9a8e09f2761c662d1ce95e5d3e829a07ea2b619b5e35e6`  
		Last Modified: Fri, 24 Apr 2020 00:05:11 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ba293916f1b61d0eee5c397f11e2e206ffaa0c54d17f2bfb328da7e6f09743`  
		Last Modified: Fri, 24 Apr 2020 00:05:10 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c6b2f1f5d52cfbabf244af757effe7b6ddc142acdb15ef5d8dc7452a9659b795
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.9 MB (316942094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516ec248376a670b87153cbe61efb69b30615826ae2ec1ee48034a951a771e92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:47:15 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:47:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:11:43 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:14:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:14:23 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:14:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:14:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:14:31 GMT
WORKDIR /go
# Tue, 14 Apr 2020 19:02:05 GMT
WORKDIR /src
# Tue, 14 Apr 2020 19:02:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 14 Apr 2020 19:02:10 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:02:15 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 14 Apr 2020 19:02:17 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 14 Apr 2020 19:03:31 GMT
RUN go get -d ./...
# Tue, 14 Apr 2020 19:03:39 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 14 Apr 2020 19:03:41 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c66f8509bb56e1ead748baf3433dcad3c1fa170146d5d7d06506b9a80f367`  
		Last Modified: Mon, 23 Mar 2020 23:53:18 GMT  
		Size: 300.6 KB (300602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf5f16b98b20e6e4f07e24e93de1018e88310a49963dc147c370d360a02fdbb`  
		Last Modified: Mon, 23 Mar 2020 23:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a38fd97575c34aedd91676d7643f6dbf66a1bca83f7d010e631807b96dae74`  
		Last Modified: Wed, 08 Apr 2020 23:25:03 GMT  
		Size: 127.8 MB (127774109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61bd435de55167e1a5a8cbdd73838375b819c98df2c23be5991140c00cbfd9a`  
		Last Modified: Wed, 08 Apr 2020 23:24:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a743cd83ba00508dd353a743708e6e434e2f56a1abdc6f2156d953839d646a1`  
		Last Modified: Tue, 14 Apr 2020 19:04:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8928c849f33d759a505e159745da8960d19460b8735d7a08631ee817549c57d5`  
		Last Modified: Tue, 14 Apr 2020 19:04:11 GMT  
		Size: 7.0 MB (7010480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe4dbb3884a7fa0c551818da659e9c4d3f97f13eb6d53634655e97f9bd2f0d`  
		Last Modified: Tue, 14 Apr 2020 19:04:10 GMT  
		Size: 2.6 MB (2584042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb4bc7d74da5ae926bd30beea4c4abe59b6c0bb76705fb4f6b83391b591ecd7`  
		Last Modified: Tue, 14 Apr 2020 19:04:53 GMT  
		Size: 176.9 MB (176851243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fb3f4c0251d63ed371fb8a24333c2d9f9dada8830bad6af323550a4276f828`  
		Last Modified: Tue, 14 Apr 2020 19:04:09 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fcea70e4e7db2fed8fb230f66d27fc46446054a0cdc6f6a342235480e7a248`  
		Last Modified: Tue, 14 Apr 2020 19:04:07 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:75a990032363651bf7b39167b9e44e70cb8e6d4ae814545a2274a74005ce8660
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317221628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb140d2ac2499d88e26b91f2219f57edca78ae1597261d9799cb9519bf9f2e24`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:58:12 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 22:58:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:11:00 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:13:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:13:19 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:13:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:13:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:13:22 GMT
WORKDIR /go
# Tue, 14 Apr 2020 19:02:03 GMT
WORKDIR /src
# Tue, 14 Apr 2020 19:02:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 14 Apr 2020 19:02:08 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Tue, 14 Apr 2020 19:02:12 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 14 Apr 2020 19:02:13 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 14 Apr 2020 19:03:13 GMT
RUN go get -d ./...
# Tue, 14 Apr 2020 19:03:15 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 14 Apr 2020 19:03:21 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d4106c43952870e20bfb808275012c22e6244af6eff1e916f446f7d338d0d`  
		Last Modified: Mon, 23 Mar 2020 23:03:34 GMT  
		Size: 301.8 KB (301778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f0a4e33d457336c22ac08eaec4609be330959ccdfefdb342be1045df4d26f0`  
		Last Modified: Mon, 23 Mar 2020 23:03:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44acbbdbf71f1d00fa6d0011bb10b82bef26b421a579bcf3a3491dced9f8233e`  
		Last Modified: Wed, 08 Apr 2020 23:21:31 GMT  
		Size: 126.4 MB (126405787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d054599df8f57e1578fdc2c554a9ac6124bf04f808dc623ef7f6548230fa3b5f`  
		Last Modified: Wed, 08 Apr 2020 23:20:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcee4e573bebbed33479e125fd8abf1f3debd0a7aee2137f55b67d9c38a79be`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968260b321a071a55eb891faac5f738bc2c3340a7843fc9ebd092902475f6fb3`  
		Last Modified: Tue, 14 Apr 2020 19:03:59 GMT  
		Size: 8.4 MB (8353090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f7e47a5a4e440d1d8c40f1b42638e70ea0fbf9b5635f0145f58768993763d6`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 2.6 MB (2584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e682841e5eb376ed223cc26d628878cb76d53d943e6f205310f7294f212717`  
		Last Modified: Tue, 14 Apr 2020 19:04:33 GMT  
		Size: 176.9 MB (176852681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdb1a37f36e66ea176ba211db0396ddcf52e5c11bc8c335ad3814c1f091f33`  
		Last Modified: Tue, 14 Apr 2020 19:03:58 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d540e0414cc6a26d9aed38f141af756f0c60e88bb278d4807bda8d6b5939314`  
		Last Modified: Tue, 14 Apr 2020 19:03:57 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:f2f734c7a8369ac0b1ffdb284f52db7b28812712357185beec2c308730fc4d10
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
$ docker pull caddy@sha256:30abbbfe8151fa239f51cf9cb5ed51c705e7b016591de1a5cba1cbe596dd2ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15155960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9477d0c347fd32b124a4d4dc0c3270d2453f7b118b3d607731e3f220da3f05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:19:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:19:25 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:19:27 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:20 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:20 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:20 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:22 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c895336717654d7bf50758d2fe590a60610eb7d7168d12c6b6bb9887bae481d`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 318.6 KB (318556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e769246751713852fe7f4107628f489ad3068e3ef3d9180d8f282591fce3ae2`  
		Last Modified: Thu, 16 Apr 2020 00:19:44 GMT  
		Size: 5.8 KB (5764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555f6fbb196736d103501b827439a43d1a6cba20ebff7df44f228f1798eb4ee`  
		Last Modified: Tue, 21 Apr 2020 00:24:36 GMT  
		Size: 12.0 MB (12028385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7ed08e071a11d38b7be1d9b2d68d6d15786980e2e6e1ee063e89493eb898a1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14409137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7460066cc8bd6b931cb96fcc0c855c2673b7923e5084718508000e664d50df61`
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
# Thu, 23 Apr 2020 17:42:34 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 23 Apr 2020 17:42:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 23 Apr 2020 17:42:40 GMT
VOLUME [/config]
# Thu, 23 Apr 2020 17:42:41 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:42:41 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 23 Apr 2020 17:42:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 23 Apr 2020 17:42:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 23 Apr 2020 17:42:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 23 Apr 2020 17:42:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 23 Apr 2020 17:42:46 GMT
EXPOSE 80
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 443
# Thu, 23 Apr 2020 17:42:47 GMT
EXPOSE 2019
# Thu, 23 Apr 2020 17:42:48 GMT
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
	-	`sha256:06e7b1f9bee864c12dd2ceef4062aa39220c9921e53de9328e46201a9706536f`  
		Last Modified: Thu, 23 Apr 2020 17:43:11 GMT  
		Size: 11.5 MB (11464427 bytes)  
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
$ docker pull caddy@sha256:b4580ebabc4eed91b683f0980d117998aca158f6690e0e8f5e09771d48aa2fbf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14115062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659da137a1ca66bfa07139e8c1504fbdf9c0915f071736c4c42fa0fc091eeb63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Thu, 16 Apr 2020 00:39:33 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 16 Apr 2020 00:39:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 16 Apr 2020 00:39:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Thu, 16 Apr 2020 00:39:36 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88' ;; 		armhf)   binArch='armv6'; checksum='5f1485c4be4a050dc12a42d9cc6b0a215a27173eca0bd46c09a0e5ac941b863511f695ca1fad211fb7ebb21e516c549aa2b6d7bc7b11ce3f3729a6c632315937' ;; 		armv7)   binArch='armv7'; checksum='f38d32e6c48f6eb889d7f7bca9ef18d953aeafe8f6ae5b37a657318890c806999dbf4161ac3f5ccb7c6b356ffbded61228e24e6b1ad5e76b3d694923c2483984' ;; 		aarch64) binArch='arm64'; checksum='c4786c030121519ea988ad418878f29b90487357bb434f357955a5ac158460192b4da136fd6d08a2507521a2920412ffa294bf2d83c858c3d1e7fb02de1482a2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 21 Apr 2020 00:24:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 21 Apr 2020 00:24:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 21 Apr 2020 00:24:35 GMT
VOLUME [/config]
# Tue, 21 Apr 2020 00:24:36 GMT
VOLUME [/data]
# Tue, 21 Apr 2020 00:24:37 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Tue, 21 Apr 2020 00:24:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 21 Apr 2020 00:24:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 21 Apr 2020 00:24:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 21 Apr 2020 00:24:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 21 Apr 2020 00:24:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 21 Apr 2020 00:24:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 21 Apr 2020 00:24:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 21 Apr 2020 00:24:49 GMT
EXPOSE 80
# Tue, 21 Apr 2020 00:24:51 GMT
EXPOSE 443
# Tue, 21 Apr 2020 00:24:52 GMT
EXPOSE 2019
# Tue, 21 Apr 2020 00:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8769f63ec8b31f05ebb26b0a58d55301ef35d1449a5f401e24fbd8fc966bfd21`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 319.1 KB (319126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaac47c6de0ab38444a53999b472ae63772dbb66155e37fc5014ee3f99d596e`  
		Last Modified: Thu, 16 Apr 2020 00:40:10 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8eecc840bde75e030ca92b955c6466f7017e33fa7a48c96d5abb6b1473e778`  
		Last Modified: Tue, 21 Apr 2020 00:25:16 GMT  
		Size: 11.1 MB (11066952 bytes)  
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

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:844b493cfdc844bf46ee328445e730513b81ca771a0b425f90381f2cd315102e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1158; amd64

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

### `caddy:windowsservercore` - windows version 10.0.14393.3630; amd64

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

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:9efbf07db38c66e53ee0497ba8229156e6ebc26a070d2fbddbdf6f6be715e5ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1158; amd64

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

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:540bc831c83dfe88a9d469750f2d8228fd14627e1cb6433a4e6b9470190c505e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

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
