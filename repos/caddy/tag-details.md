<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.2.1`](#caddy221)
-	[`caddy:2.2.1-alpine`](#caddy221-alpine)
-	[`caddy:2.2.1-builder`](#caddy221-builder)
-	[`caddy:2.2.1-builder-alpine`](#caddy221-builder-alpine)
-	[`caddy:2.2.1-builder-windowsservercore-1809`](#caddy221-builder-windowsservercore-1809)
-	[`caddy:2.2.1-builder-windowsservercore-ltsc2016`](#caddy221-builder-windowsservercore-ltsc2016)
-	[`caddy:2.2.1-windowsservercore`](#caddy221-windowsservercore)
-	[`caddy:2.2.1-windowsservercore-1809`](#caddy221-windowsservercore-1809)
-	[`caddy:2.2.1-windowsservercore-ltsc2016`](#caddy221-windowsservercore-ltsc2016)
-	[`caddy:2.3.0`](#caddy230)
-	[`caddy:2.3.0-alpine`](#caddy230-alpine)
-	[`caddy:2.3.0-builder`](#caddy230-builder)
-	[`caddy:2.3.0-builder-alpine`](#caddy230-builder-alpine)
-	[`caddy:2.3.0-builder-windowsservercore-1809`](#caddy230-builder-windowsservercore-1809)
-	[`caddy:2.3.0-builder-windowsservercore-ltsc2016`](#caddy230-builder-windowsservercore-ltsc2016)
-	[`caddy:2.3.0-windowsservercore`](#caddy230-windowsservercore)
-	[`caddy:2.3.0-windowsservercore-1809`](#caddy230-windowsservercore-1809)
-	[`caddy:2.3.0-windowsservercore-ltsc2016`](#caddy230-windowsservercore-ltsc2016)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2016`](#caddy2-builder-windowsservercore-ltsc2016)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:builder-windowsservercore-ltsc2016`](#caddybuilder-windowsservercore-ltsc2016)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2016`](#caddywindowsservercore-ltsc2016)

## `caddy:2`

```console
$ docker pull caddy@sha256:925100cc9e08c8d79ee37b36abe21d2f554982d5bf302c55a38f5da971f53431
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:cbb1e84121ca20ac7fbc3cf8a9e04f4ee4979f33352ecfb883b56984fccf2cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73dc9258a8ebf0244d67701a655c1fc655cbfda642ab615e06b1a6039d5b2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:19:40 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:19:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:19:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:19:43 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:46 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe9aaa681bd550de2455df437d9c9a9e24005e810e7d5a01c35d263fa2aa46`  
		Last Modified: Mon, 04 Jan 2021 18:20:23 GMT  
		Size: 11.6 MB (11622354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3b11169846dc2fcfacfbcaae13fcc50c8b72dc70b6bc9c4cfd9f156a37c4c`  
		Last Modified: Mon, 04 Jan 2021 18:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b11903d75dc786cc7a333dcc8eb86432e12286a27596ba9a13de8ce6a16bbe4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f2d0ff6672d884939bbd0e7ae29c28c4a54054bfb0132b16a6fd7144ccf4d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:49:38 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:49:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:49:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:49:46 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:49:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:49:51 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:49:53 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:49:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493ce1c2e0e02619db2817c3da32453658bbca2b087c8d73cf9c8eae72e5926`  
		Last Modified: Mon, 04 Jan 2021 18:50:38 GMT  
		Size: 10.9 MB (10944839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a640f55dfe60d817bb1c48cf163e52c3c42b843b7aa9976d573ac5b4bb322a04`  
		Last Modified: Mon, 04 Jan 2021 18:50:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8d7dd8d7f22f669d44669e643d61092c90ec7c1bcd4704e119d72715dc4b7de1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8ff470d547b26a0bf496261541723024fa700eb9d162dad5eba091a1320ce5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:57:42 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:57:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:57:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:57:49 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:57:49 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:57:50 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:57:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:57:57 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:57:58 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1178be4a6bd4aee0a16e25358732f4deac6a84f6614bd4d5a9d242ac9068d`  
		Last Modified: Mon, 04 Jan 2021 18:58:43 GMT  
		Size: 10.9 MB (10925337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb438ac85eaa28804b9de2f3e230fe52916ba5b81a38b03c514f2dbe9282c679`  
		Last Modified: Mon, 04 Jan 2021 18:58:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93f5ca2902036950ab4ab8a22f4d74f36bce55feee9b7e0e797396e2d07f4df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9774262cda02b94b5c9cc6bfc57d947819c3a0f1e85aacb278c6e91ddd7850`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:39:58 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:40:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:40:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:40:03 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:40:04 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:40:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:40:17 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:40:18 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:40:19 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:40:19 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48312421be65c130b3524264024f10c7774e9eab1b9cf370a6c7022753927567`  
		Last Modified: Mon, 04 Jan 2021 18:41:12 GMT  
		Size: 10.6 MB (10598984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332c70787e2588f66eeb0b6abd933d1f004e4f0357a5618092fdb36f9e88913f`  
		Last Modified: Mon, 04 Jan 2021 18:41:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:1be56543a90159f9a8bd5a83094c762bda8baef783604503316fcafbc5467c09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13354933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b014a3125a542b761c87a24c6c1c5f71f964b4414c310af9ce20822717a8e2ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:17:34 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:18:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:18:12 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:18:18 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:18:23 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:18:29 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:18:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:27 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:43 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:50 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:55 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecaad708cba83777a49b8b0153fd11aa1fda8c3de8c2669359510c7fba8e1d4`  
		Last Modified: Mon, 04 Jan 2021 18:21:19 GMT  
		Size: 10.2 MB (10241384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235fec692a51bccc1545ea1f8f892604e9198ae61248e12ddeba4043bea2c1f3`  
		Last Modified: Mon, 04 Jan 2021 18:21:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:1d605f274d1eca015a6899f98aed7e87ddbcf21fee25db45eb3af04b7fa35c7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a2f900066e27e26138f6cac769b05f6cd3b0c6859052c1aa39eba8665d1a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:41:41 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:41:47 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:41:48 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e914cfc82e9092a831f17f5daebbbde8ebe39d7fe50230325ce80f657bfe3f0f`  
		Last Modified: Mon, 04 Jan 2021 18:42:29 GMT  
		Size: 11.3 MB (11272057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d554de8138d32421dfdcb23f0feec824f7106586791ae523f39943c710ad71`  
		Last Modified: Mon, 04 Jan 2021 18:42:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1`

```console
$ docker pull caddy@sha256:6bb9d303dcd6b846e36467ff187c01c6a1a026eb4ea5b76919b8d100d1faa3e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.2.1` - linux; amd64

```console
$ docker pull caddy@sha256:6c52994f26f7f3fd5db685627f6dae43b2bec3769718ded39da8a8399081dc1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14637432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e3eab0f95d34ce20778d55ab14e5acf2a9dcc58e51ac68d79080d6e13af10e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 12:35:29 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 12:35:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 12:35:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 12:35:34 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 12:35:34 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 12:35:35 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 12:35:35 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 12:35:35 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 12:35:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 12:35:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 12:35:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 12:35:37 GMT
EXPOSE 80
# Thu, 17 Dec 2020 12:35:37 GMT
EXPOSE 443
# Thu, 17 Dec 2020 12:35:37 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 12:35:37 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 12:35:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093aa05efcd0222180018f9b0b7f692f498643f2cca89879f710281ef4eb82f4`  
		Last Modified: Thu, 17 Dec 2020 12:36:49 GMT  
		Size: 11.5 MB (11532503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e6e211c46dbac2746ba2129f181597529ef0786c8291a1e008597b2b22b987`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:600f49e71300192bf31ea677700c97e1378e1e538382e8c6f4866df172d6c7fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5d5ebcfb556749a17900eda13204b051daa0314a3e2b973f91477639b8bba9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 00:58:07 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 00:58:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 00:58:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:58:13 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 00:58:14 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 00:58:15 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 00:58:15 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 00:58:16 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 00:58:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 00:58:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 00:58:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 00:58:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 00:58:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 00:58:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 00:58:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 00:58:21 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:58:22 GMT
EXPOSE 443
# Thu, 17 Dec 2020 00:58:22 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 00:58:23 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 00:58:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9987cfec761415ed2b93a97e9b9f4a4697e17fa62918c4d605b07575dc0b26f6`  
		Last Modified: Thu, 17 Dec 2020 00:59:54 GMT  
		Size: 10.9 MB (10876277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c751e5903dd026412f8022a397eae3a5e8bfc230cd0aa7f7ebdd0df790797d44`  
		Last Modified: Thu, 17 Dec 2020 00:59:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd11025259b8f4e5ff0fb4be850687ffb0867a2d9944abde71eabc0d1f960c3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13567123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:886b42d48a4a2ecf2c76c3f5b87dc686c0ed1a6825148b55a52412aec45534b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 01:02:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 01:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 01:03:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:03:09 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 01:03:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 01:03:12 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 01:03:13 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 01:03:14 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 01:03:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 01:03:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 01:03:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 01:03:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 01:03:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 01:03:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 01:03:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 01:03:25 GMT
EXPOSE 80
# Thu, 17 Dec 2020 01:03:26 GMT
EXPOSE 443
# Thu, 17 Dec 2020 01:03:27 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 01:03:29 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 01:03:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f35c06f256db819c11f6fedc7891e6d3d113cbf8ccc842ce7aa8dc2297ddf9`  
		Last Modified: Thu, 17 Dec 2020 01:05:15 GMT  
		Size: 10.9 MB (10854396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f49080ad39809ab25c77896f4ae175774ddb90803b62c4cff40993a5dc5ea2e`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:433c4bdf6ee2160e8ad5ea514f38d504f28175cb6962c4fe9df08b9c7e106572
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13542834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c97501c8ae3d24c0dfbd4f07bbb657b810d06822a3f705e34ab925ee0af135`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 00:33:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 00:33:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:33:44 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 00:33:46 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 00:33:47 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 00:33:48 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 00:33:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 00:33:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 00:33:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 00:33:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 00:33:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 00:33:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 00:33:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 00:33:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 00:33:56 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:33:57 GMT
EXPOSE 443
# Thu, 17 Dec 2020 00:33:58 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 00:33:59 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 00:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dae80642a26e64bdb4950988ad132509f4e762b2112e54cf4a01e53a7d20940`  
		Last Modified: Thu, 17 Dec 2020 00:35:44 GMT  
		Size: 10.5 MB (10527464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a133d29fd2bcb955f4cad5ab4987986adb395f599eb0670e05548a6fabac9d6c`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:2b98157d368e34be38c52250051c9b1ef1c9c2e1cdf7ad689cb787114ed81c8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13293774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde80cd55aa83872b68b6431b786874187b380c2b9e6e76bec6f88aff0899c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 02:29:12 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 02:29:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 02:29:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 02:29:34 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 02:29:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 02:29:39 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 02:29:43 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 02:29:47 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 02:29:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 02:29:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 02:29:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 02:30:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 02:30:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 02:30:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 02:30:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 02:30:42 GMT
EXPOSE 80
# Thu, 17 Dec 2020 02:30:50 GMT
EXPOSE 443
# Thu, 17 Dec 2020 02:30:57 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 02:31:05 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 02:31:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49ef37f5d37e271fe0c59da9bf646cddcf531288af8e7bd1dcc2f19f00512fa`  
		Last Modified: Thu, 17 Dec 2020 02:34:50 GMT  
		Size: 10.2 MB (10180225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4232127c642a135916049f992dd74e604e5d3209ecb9e4ef03a0cec10919c19`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - linux; s390x

```console
$ docker pull caddy@sha256:1cac96282fb670437569c18cecd2134488d0866a91814c535a678f50fd7a5b31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14076023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d8b1034a1b47231587f5206d8e6183e7b4d86c17d0b25ddd87206b20dd01d5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 00:26:24 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 00:26:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 00:26:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:26:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 00:26:34 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 00:26:34 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 00:26:35 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 00:26:36 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 00:26:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 00:26:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 00:26:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 00:26:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 00:26:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 00:26:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 00:26:41 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:41 GMT
EXPOSE 443
# Thu, 17 Dec 2020 00:26:42 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 00:26:43 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 00:26:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43adc457038c7b112aa803714ad036b455b9ff1e529a8adeac2e03ca6c4d44`  
		Last Modified: Thu, 17 Dec 2020 00:28:19 GMT  
		Size: 11.2 MB (11202562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2def3ab9ebb3191504a570a553030e4f3c2962cb8d451f4a5215c3ec29c81e5`  
		Last Modified: Thu, 17 Dec 2020 00:28:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:6da1bf1d8a609cef807ec4b7a3ad098a98655b240f92a1cedc0060c45c7bdb52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465382060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f096f4d4e87096ef9f385ee497d55a6e50fd022edf1d255d2dd3235578e1f18`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:42:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:42:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:43:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:43:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:43:01 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:43:02 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:43:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 10 Feb 2021 19:43:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:43:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:43:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:43:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:43:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:43:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:43:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:43:08 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:43:09 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:43:10 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:43:25 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:43:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfcfa417a148200a9b82e1221d8bf8897b6b076efa05274d844d5c53829055f`  
		Last Modified: Wed, 10 Feb 2021 19:55:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36838d8cd4839ff406029e6bb1522cf44be6fbe6c7467921e5248b6c07a6aff5`  
		Last Modified: Wed, 10 Feb 2021 19:55:24 GMT  
		Size: 16.4 MB (16355614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e0f9d5139c635a9b975de4e63ad4f189516074a29dc56dd6d8fb7d277f433c`  
		Last Modified: Wed, 10 Feb 2021 19:55:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b851528d2df67a7c64ba6ffdffa9c9d295d9138c2118aa97ecb314bf8df40f31`  
		Last Modified: Wed, 10 Feb 2021 19:55:18 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abf701bca17610cfb13a04514ce3c1ae42cb17492484e2d3a1bce2a993a0f2f`  
		Last Modified: Wed, 10 Feb 2021 19:55:17 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f098af20d8519222d42bd836d1471d98ee831d2d922b13f7ca3c0b653c17f`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4267ee0ca74419bceecbf19e1465e0932bf90853f3268cfd144b6db60b8641`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f70a85d3b2f625c056ad12065547cd237ef4b5ae8a60449a5e85117837dcd4`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac9e58e231ffaac8a880d0de3eba5b4c2851b6a2a536719a3f3e45a660dd356`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d12c4db5395f443755c890788da47b44c0d59b25175fc18d1b0bcbca76f16c`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad520c9c3b5f0572b6c0ce26ef18a5ff0713f07f11a46974fd48597878e9da6`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef810b81f96651a0d2a0343fd3900d50c9f202fe114d740491fe64ea12c23815`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4c4b552633a82d1828c5cf24c2b3296792f992f6adae82c355822dbab99fd3`  
		Last Modified: Wed, 10 Feb 2021 19:55:13 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56267262030645aab5169f5cb94219ebbfe0427ab3d8f651e64956698f456`  
		Last Modified: Wed, 10 Feb 2021 19:55:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cfc4cbe95dd30bb06e52b3c2eaff805f74390d6241725fb431e28f21b0b988`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4e650a14400b1015308d7f542896c289c208edaa9b67dcc7c7c267290721cc`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d8f608756523415340070b95c5c66d516ab5ce49761a6d52f3c4bb374ceaab`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70036fc946d8c35838e5156a1cdbc4acfa0dfb7777e8a2b1c68c3575cabb773`  
		Last Modified: Wed, 10 Feb 2021 19:55:11 GMT  
		Size: 309.8 KB (309825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53eae9f2023fc3b9116bfae51eaad4e7a8eb05e67e9a03b8060a647e4cc47546`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:8f8fc4ea6e1563ee3ab2e75f793d715f62337829fa749303166f4c7b87b5fd6d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827259946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0764db061b485b056f35a9f55f331c66b513a6d4f5c94880eeb19647e3a07a6a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:44:53 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:46:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:46:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:46:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:46:17 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:46:18 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:46:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 10 Feb 2021 19:46:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:46:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:46:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:46:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:46:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:46:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:46:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:46:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:46:25 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:46:26 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:47:11 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:47:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0153fb9a550966fcb9a46155ee3f854d53cc8f5b93fd222e527469f624ed3864`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2428d9ebac128c1e235ea0193b3c686f3ac2ab39cab995e1c8950c8ba8337108`  
		Last Modified: Wed, 10 Feb 2021 19:55:52 GMT  
		Size: 21.8 MB (21775071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73e38964af26f07515595914dbb34cd08962428af69bf0f79a6c0acdb12df0`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2afd55956abba10688ff7bfcf894ee904de66d652a57b38f45d817ea24970f`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c40aa362fe3f06b3f8c638f3854b0003e87e83183e2d8255a4862257ec52aa5`  
		Last Modified: Wed, 10 Feb 2021 19:55:44 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cfeb85cad3ac53abec8be2a3433b84c7f3f596ea01b2bfd233a4d9604ddae5`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390c6e6af32e283bc45b0c07174103c4263221fa41133a3fb2e755338192a4db`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff06a60beba4f6825ecedb53f80e24c9c840cefc4a1e5d8e209caee2e93fd28e`  
		Last Modified: Wed, 10 Feb 2021 19:55:44 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761310cffade38a82d35d76a24350f795a0be62f747f960091dc6d74a9e42a4`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04119ba7d167513dc8fced1f79bd470007be8ea9e8cf3e7a61a57bdb2c9e437b`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcde858b06f73f425ae981873771bd224454ae0a366f3a03c03fa98c5866525d`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dcd0be1c9074d48807389fdb9bd95dd690cf6019fc42334d0a791b8a5a7941`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a62a5e70c867b79ba59a6ea275147b03ca5b486f341a045864fac3863beebb`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8878b460a7cfd33f71877a734283e4595adbd16400d59851fa802ce0a9a5d93`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b19f25838b5e2e96f5e8fe1bb366280f0c88b8fc1855eeb9b140a01c8ebc45`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1cabc58724baadec9cca0c08a3c1833f0179349372ce8115bf36021272f3f4`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b54c44ea72868954c9879ee9eefed550ba0bb56079307558f1c36b31f3147d`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb3bd379edf42c402d41f0d72f4ce290ff35087f1ff4d69d91c756fd113106c`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 267.8 KB (267828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5514ed308f579e66e3c855f9598400c11f48dfbd4719fd00c8ed95b852c8b9b9`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-alpine`

```console
$ docker pull caddy@sha256:e9c4066bde43f17c060ec9904f56ba503caa84384f81fafa1f75d8b52b52d6d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6c52994f26f7f3fd5db685627f6dae43b2bec3769718ded39da8a8399081dc1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14637432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e3eab0f95d34ce20778d55ab14e5acf2a9dcc58e51ac68d79080d6e13af10e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 12:35:29 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 12:35:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 12:35:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 12:35:34 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 12:35:34 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 12:35:35 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 12:35:35 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 12:35:35 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 12:35:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 12:35:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 12:35:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 12:35:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 12:35:37 GMT
EXPOSE 80
# Thu, 17 Dec 2020 12:35:37 GMT
EXPOSE 443
# Thu, 17 Dec 2020 12:35:37 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 12:35:37 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 12:35:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093aa05efcd0222180018f9b0b7f692f498643f2cca89879f710281ef4eb82f4`  
		Last Modified: Thu, 17 Dec 2020 12:36:49 GMT  
		Size: 11.5 MB (11532503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e6e211c46dbac2746ba2129f181597529ef0786c8291a1e008597b2b22b987`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:600f49e71300192bf31ea677700c97e1378e1e538382e8c6f4866df172d6c7fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5d5ebcfb556749a17900eda13204b051daa0314a3e2b973f91477639b8bba9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 00:58:07 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 00:58:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 00:58:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:58:13 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 00:58:14 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 00:58:15 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 00:58:15 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 00:58:16 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 00:58:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 00:58:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 00:58:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 00:58:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 00:58:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 00:58:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 00:58:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 00:58:21 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:58:22 GMT
EXPOSE 443
# Thu, 17 Dec 2020 00:58:22 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 00:58:23 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 00:58:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9987cfec761415ed2b93a97e9b9f4a4697e17fa62918c4d605b07575dc0b26f6`  
		Last Modified: Thu, 17 Dec 2020 00:59:54 GMT  
		Size: 10.9 MB (10876277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c751e5903dd026412f8022a397eae3a5e8bfc230cd0aa7f7ebdd0df790797d44`  
		Last Modified: Thu, 17 Dec 2020 00:59:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd11025259b8f4e5ff0fb4be850687ffb0867a2d9944abde71eabc0d1f960c3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13567123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:886b42d48a4a2ecf2c76c3f5b87dc686c0ed1a6825148b55a52412aec45534b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 01:02:57 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 01:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 01:03:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:03:09 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 01:03:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 01:03:12 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 01:03:13 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 01:03:14 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 01:03:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 01:03:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 01:03:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 01:03:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 01:03:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 01:03:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 01:03:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 01:03:25 GMT
EXPOSE 80
# Thu, 17 Dec 2020 01:03:26 GMT
EXPOSE 443
# Thu, 17 Dec 2020 01:03:27 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 01:03:29 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 01:03:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f35c06f256db819c11f6fedc7891e6d3d113cbf8ccc842ce7aa8dc2297ddf9`  
		Last Modified: Thu, 17 Dec 2020 01:05:15 GMT  
		Size: 10.9 MB (10854396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f49080ad39809ab25c77896f4ae175774ddb90803b62c4cff40993a5dc5ea2e`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:433c4bdf6ee2160e8ad5ea514f38d504f28175cb6962c4fe9df08b9c7e106572
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13542834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c97501c8ae3d24c0dfbd4f07bbb657b810d06822a3f705e34ab925ee0af135`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 00:33:34 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 00:33:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 00:33:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:33:44 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 00:33:46 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 00:33:47 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 00:33:48 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 00:33:48 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 00:33:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 00:33:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 00:33:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 00:33:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 00:33:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 00:33:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 00:33:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 00:33:56 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:33:57 GMT
EXPOSE 443
# Thu, 17 Dec 2020 00:33:58 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 00:33:59 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 00:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dae80642a26e64bdb4950988ad132509f4e762b2112e54cf4a01e53a7d20940`  
		Last Modified: Thu, 17 Dec 2020 00:35:44 GMT  
		Size: 10.5 MB (10527464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a133d29fd2bcb955f4cad5ab4987986adb395f599eb0670e05548a6fabac9d6c`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:2b98157d368e34be38c52250051c9b1ef1c9c2e1cdf7ad689cb787114ed81c8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13293774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde80cd55aa83872b68b6431b786874187b380c2b9e6e76bec6f88aff0899c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 02:29:12 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 02:29:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 02:29:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 02:29:34 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 02:29:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 02:29:39 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 02:29:43 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 02:29:47 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 02:29:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 02:29:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 02:29:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 02:30:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 02:30:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 02:30:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 02:30:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 02:30:42 GMT
EXPOSE 80
# Thu, 17 Dec 2020 02:30:50 GMT
EXPOSE 443
# Thu, 17 Dec 2020 02:30:57 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 02:31:05 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 02:31:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49ef37f5d37e271fe0c59da9bf646cddcf531288af8e7bd1dcc2f19f00512fa`  
		Last Modified: Thu, 17 Dec 2020 02:34:50 GMT  
		Size: 10.2 MB (10180225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4232127c642a135916049f992dd74e604e5d3209ecb9e4ef03a0cec10919c19`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1cac96282fb670437569c18cecd2134488d0866a91814c535a678f50fd7a5b31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14076023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d8b1034a1b47231587f5206d8e6183e7b4d86c17d0b25ddd87206b20dd01d5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 17 Dec 2020 00:26:24 GMT
ENV CADDY_VERSION=v2.2.1
# Thu, 17 Dec 2020 00:26:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='66a21e0643fd2538ffe88ab93cb4a158b94873c1ce7494543a8355c8a3492d5fa43f4fa030dfc9e9833d15fe04f010063c61cb3f04ad5ac6bcff80396f928a08' ;; 		armhf)   binArch='armv6'; checksum='7e358d452fe7bbc0cdcba8a800339e34bd6277f698909d1d7a3b2ebd722653899b9bff6b7e8b996e9f054356374537f9971c1d5aed95f117dcce6be08e80446e' ;; 		armv7)   binArch='armv7'; checksum='ed847f91c9726ba4f25dbf9954ebe072c893f3eecfac3b83ee5c541fc762f88f59b4bd8aa35d54dd1ac043ca6e54235a197137529fe003792fdc3801a5100cd0' ;; 		aarch64) binArch='arm64'; checksum='dfc7ef12feea26b13b818cac8492664662c24835db1f8b862500debfddd30b7399d3ccc18a52fc8cc62b82ddb4cc41f2810580c1727b6c22e27dd74724bfae96' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3b38fcb4752be955e05156d2510825e93c7f83592a405d22f9ecd63cecd1d102b2aae4b50ce8586c035edd5d53075d4daeac986bc2cc1e2e1f41c6d9723066c5' ;; 		s390x)   binArch='s390x'; checksum='ebd76de742d38556aa6a7c68c000d530f46989f3db712b486d4dbe653ca69c3ba2333d19337e85d63c619f5c410f1d22dc982d9cdb6ce5e1ed94dbf29ec15190' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Dec 2020 00:26:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 00:26:33 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Dec 2020 00:26:34 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Dec 2020 00:26:34 GMT
VOLUME [/config]
# Thu, 17 Dec 2020 00:26:35 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 00:26:36 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Thu, 17 Dec 2020 00:26:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Dec 2020 00:26:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Dec 2020 00:26:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Dec 2020 00:26:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Dec 2020 00:26:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Dec 2020 00:26:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Dec 2020 00:26:41 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:41 GMT
EXPOSE 443
# Thu, 17 Dec 2020 00:26:42 GMT
EXPOSE 2019
# Thu, 17 Dec 2020 00:26:43 GMT
WORKDIR /srv
# Thu, 17 Dec 2020 00:26:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43adc457038c7b112aa803714ad036b455b9ff1e529a8adeac2e03ca6c4d44`  
		Last Modified: Thu, 17 Dec 2020 00:28:19 GMT  
		Size: 11.2 MB (11202562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2def3ab9ebb3191504a570a553030e4f3c2962cb8d451f4a5215c3ec29c81e5`  
		Last Modified: Thu, 17 Dec 2020 00:28:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder`

```console
$ docker pull caddy@sha256:9b8b7ccb147afabd3d7d0e7b29c0a17fd5f0c60bb9b6c86ffde3720d19a32775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.2.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:f26a8b2a4544de99f6d3b4baca56bbeb794955ab503247e583a086596bcf7144
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680f20c245fd2a119386c98ff446ff10020755f1809bb0fcec741b107248f7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 05:35:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4baddae0db2d58a149e4c0944d85e42c0549a7c59c30b0d6adbb2967e944bfc`  
		Last Modified: Fri, 05 Feb 2021 05:35:51 GMT  
		Size: 1.3 MB (1308352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424c4cdb157805bdbb1b78c3af10ff6177b5ea09fbb19a6a4c2c4c189029f447`  
		Last Modified: Fri, 05 Feb 2021 05:35:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e534d5dcab2baa57c4609a9740f7d944a8e1f9fc2b29bfa00558c233f7f75455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28803d4a208f14f6a4a4818d6aee71237a0ac9fd194f7de2bd165b99c30d973c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:26 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 02:58:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142d3d315670b05e1b2ae03d4fabab4ebc35c05aafa3929e9f2d2bda9833bbca`  
		Last Modified: Fri, 05 Feb 2021 02:59:09 GMT  
		Size: 1.2 MB (1219254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9939af82b5c796a5cc01e18e7b126451949b8072c80796a2cf788bd914dd5`  
		Last Modified: Fri, 05 Feb 2021 02:59:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8993f2d2901f9cbbc35971e19622200b5ae3673fda17fd422850cc1324b99dff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51faa5fa84893e734fbacd3952f26e56fc4bc174b919d86d02cb685fc4ec505`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:25 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 04:09:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b15db0f3970b828f922daeaf9fc37d0ec99c7f7bd6edc62e8736d724a8b2e4`  
		Last Modified: Fri, 05 Feb 2021 04:10:11 GMT  
		Size: 1.2 MB (1216919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624de09fd3df566099e0a80c1d1a7bcb8d062fbdefff0a424c4b0cbcb24738fa`  
		Last Modified: Fri, 05 Feb 2021 04:10:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:521f512c39e332bdc7d9b2e20810a13fe14b66c891f02ecf79f0836bb9ab522d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682b38912be519a5a6e3f7375be526cb32754b8d3281ca10215ab47b2f238c98`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:00:59 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 04:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d9715bd4a76d86863a98ef7410e8c1ee8ef3b4edbd91f91cfdc59ccf6f20da`  
		Last Modified: Fri, 05 Feb 2021 04:01:52 GMT  
		Size: 1.2 MB (1199521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c73c681c71efac3993719db74e6cd364100dfc2864348755eeb8a433edbfc5`  
		Last Modified: Fri, 05 Feb 2021 04:01:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:0291da7af5b30eb0daef4f4be75d0e9342548458ca7ca4f3847ffde4224cb636
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d97c61bd86075443ff8bf19d20e3af28ec8cc7b02959309335035e27d8794fe7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:03:53 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 12:04:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:04:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:04:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:04:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ded8f2072b2783f42b3ec943a4ccbba05ca46671a1c54879c1400aa799289fe`  
		Last Modified: Fri, 05 Feb 2021 12:05:51 GMT  
		Size: 1.2 MB (1168988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f607ae36e335adcf95d40dda3490d418bcc95d43d46456fac355992e2f7ba42`  
		Last Modified: Fri, 05 Feb 2021 12:05:51 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:69cf58f13e0ebbae8397cc38d5dbae53a5ebbadc77ca2a2d5d5a0c5d6e9384eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c022b0a2e1b6d9cdc3204e573e594ab547231613a413ece8e12233033de26b18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:44:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 11:44:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:44:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:44:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:44:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952d0aa0aa02aa19be72e36c3000c39d72042bb8102893b4f3282ea08c0d1ddf`  
		Last Modified: Fri, 05 Feb 2021 11:46:12 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba264217340623f7b55afafa9e3178443f1e6a83ec3b7ef6800b2731227c9a6b`  
		Last Modified: Fri, 05 Feb 2021 11:46:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:5c377275b3dcf019e5067be45da846dc95cb559946239d05268b2df12e99bf30
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93448cf4cb6e1bf0016617d771b08c7e9e291e8fdaeff3375461b91608fbf108`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:47:17 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:47:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:47:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:47:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca886e5098a8d28a6df0a149c296aed2e089a054b02aebc21aa845fdf8e98ab4`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2018e9b1b545e69b879935b611f08e0ccb56dbae0f79b4c913110da403bee2`  
		Last Modified: Wed, 10 Feb 2021 19:56:07 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae5621b15a5cadc2b0010bcfa556a66bbf6b297eea2fa5a09b2d2c9fa7a672`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.7 MB (1707443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34455d94a729a90f7726c34bde85e5f0cf617503812d19e5e876312a62fbc3c4`  
		Last Modified: Wed, 10 Feb 2021 19:56:07 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:922aeb69e5e61d75775bdb7acb8b51870800d23786bcb0f1d50a98fb1ef6164d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991341907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1321cc626c7cc2e789bfdad59d75b76a9a1e8628d6553bccff4968d45be836de`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:47:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:47:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:49:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:49:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dfbb427057bd0320e5b06f34b6721d2dc92c5a40a740d70aeeb1e50267a84b`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3ccc20fa93d10cb74787e660a1f74234fadcbd58528928ee4654713628dcb1`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d591793f27509d36d3d1cdfe5cc9ca23584bee99813012dc7130ca866b3ce6`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 11.5 MB (11510997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d99f508d8c6990ce0baadab2e2cb01761d6ee91c2ff083f1c278b0aed2f0e2e`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-alpine`

```console
$ docker pull caddy@sha256:acb4381e0ecbc7b892cab0dff40809c8fd98c7840e9a4495b498055d7c0e8854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:f26a8b2a4544de99f6d3b4baca56bbeb794955ab503247e583a086596bcf7144
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680f20c245fd2a119386c98ff446ff10020755f1809bb0fcec741b107248f7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:13 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 05:35:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4baddae0db2d58a149e4c0944d85e42c0549a7c59c30b0d6adbb2967e944bfc`  
		Last Modified: Fri, 05 Feb 2021 05:35:51 GMT  
		Size: 1.3 MB (1308352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424c4cdb157805bdbb1b78c3af10ff6177b5ea09fbb19a6a4c2c4c189029f447`  
		Last Modified: Fri, 05 Feb 2021 05:35:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e534d5dcab2baa57c4609a9740f7d944a8e1f9fc2b29bfa00558c233f7f75455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28803d4a208f14f6a4a4818d6aee71237a0ac9fd194f7de2bd165b99c30d973c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:26 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 02:58:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142d3d315670b05e1b2ae03d4fabab4ebc35c05aafa3929e9f2d2bda9833bbca`  
		Last Modified: Fri, 05 Feb 2021 02:59:09 GMT  
		Size: 1.2 MB (1219254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9939af82b5c796a5cc01e18e7b126451949b8072c80796a2cf788bd914dd5`  
		Last Modified: Fri, 05 Feb 2021 02:59:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8993f2d2901f9cbbc35971e19622200b5ae3673fda17fd422850cc1324b99dff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51faa5fa84893e734fbacd3952f26e56fc4bc174b919d86d02cb685fc4ec505`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:25 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 04:09:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b15db0f3970b828f922daeaf9fc37d0ec99c7f7bd6edc62e8736d724a8b2e4`  
		Last Modified: Fri, 05 Feb 2021 04:10:11 GMT  
		Size: 1.2 MB (1216919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624de09fd3df566099e0a80c1d1a7bcb8d062fbdefff0a424c4b0cbcb24738fa`  
		Last Modified: Fri, 05 Feb 2021 04:10:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:521f512c39e332bdc7d9b2e20810a13fe14b66c891f02ecf79f0836bb9ab522d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682b38912be519a5a6e3f7375be526cb32754b8d3281ca10215ab47b2f238c98`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:00:59 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 04:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d9715bd4a76d86863a98ef7410e8c1ee8ef3b4edbd91f91cfdc59ccf6f20da`  
		Last Modified: Fri, 05 Feb 2021 04:01:52 GMT  
		Size: 1.2 MB (1199521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c73c681c71efac3993719db74e6cd364100dfc2864348755eeb8a433edbfc5`  
		Last Modified: Fri, 05 Feb 2021 04:01:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0291da7af5b30eb0daef4f4be75d0e9342548458ca7ca4f3847ffde4224cb636
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d97c61bd86075443ff8bf19d20e3af28ec8cc7b02959309335035e27d8794fe7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:03:53 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 12:04:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:04:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:04:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:04:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ded8f2072b2783f42b3ec943a4ccbba05ca46671a1c54879c1400aa799289fe`  
		Last Modified: Fri, 05 Feb 2021 12:05:51 GMT  
		Size: 1.2 MB (1168988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f607ae36e335adcf95d40dda3490d418bcc95d43d46456fac355992e2f7ba42`  
		Last Modified: Fri, 05 Feb 2021 12:05:51 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:69cf58f13e0ebbae8397cc38d5dbae53a5ebbadc77ca2a2d5d5a0c5d6e9384eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c022b0a2e1b6d9cdc3204e573e594ab547231613a413ece8e12233033de26b18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:44:54 GMT
ENV CADDY_VERSION=v2.2.1
# Fri, 05 Feb 2021 11:44:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:44:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:44:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:44:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952d0aa0aa02aa19be72e36c3000c39d72042bb8102893b4f3282ea08c0d1ddf`  
		Last Modified: Fri, 05 Feb 2021 11:46:12 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba264217340623f7b55afafa9e3178443f1e6a83ec3b7ef6800b2731227c9a6b`  
		Last Modified: Fri, 05 Feb 2021 11:46:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:d815ac9816cad59735808ba43f6aba1ee7b4066bedb08c4e1863d6a8ccec8457
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.2.1-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:5c377275b3dcf019e5067be45da846dc95cb559946239d05268b2df12e99bf30
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93448cf4cb6e1bf0016617d771b08c7e9e291e8fdaeff3375461b91608fbf108`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:47:17 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:47:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:47:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:47:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca886e5098a8d28a6df0a149c296aed2e089a054b02aebc21aa845fdf8e98ab4`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2018e9b1b545e69b879935b611f08e0ccb56dbae0f79b4c913110da403bee2`  
		Last Modified: Wed, 10 Feb 2021 19:56:07 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae5621b15a5cadc2b0010bcfa556a66bbf6b297eea2fa5a09b2d2c9fa7a672`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.7 MB (1707443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34455d94a729a90f7726c34bde85e5f0cf617503812d19e5e876312a62fbc3c4`  
		Last Modified: Wed, 10 Feb 2021 19:56:07 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:703fec53f01654521cf12d82ab818b920b0e78e41107682ff579dc134d9a913e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.2.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:922aeb69e5e61d75775bdb7acb8b51870800d23786bcb0f1d50a98fb1ef6164d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991341907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1321cc626c7cc2e789bfdad59d75b76a9a1e8628d6553bccff4968d45be836de`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:47:48 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:47:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:49:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:49:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dfbb427057bd0320e5b06f34b6721d2dc92c5a40a740d70aeeb1e50267a84b`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3ccc20fa93d10cb74787e660a1f74234fadcbd58528928ee4654713628dcb1`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d591793f27509d36d3d1cdfe5cc9ca23584bee99813012dc7130ca866b3ce6`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 11.5 MB (11510997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d99f508d8c6990ce0baadab2e2cb01761d6ee91c2ff083f1c278b0aed2f0e2e`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore`

```console
$ docker pull caddy@sha256:3332ccf6390d071040fd4ccb7fd1f6813746dd99a73ce3c828dd45d63f648d01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.2.1-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:6da1bf1d8a609cef807ec4b7a3ad098a98655b240f92a1cedc0060c45c7bdb52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465382060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f096f4d4e87096ef9f385ee497d55a6e50fd022edf1d255d2dd3235578e1f18`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:42:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:42:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:43:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:43:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:43:01 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:43:02 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:43:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 10 Feb 2021 19:43:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:43:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:43:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:43:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:43:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:43:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:43:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:43:08 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:43:09 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:43:10 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:43:25 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:43:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfcfa417a148200a9b82e1221d8bf8897b6b076efa05274d844d5c53829055f`  
		Last Modified: Wed, 10 Feb 2021 19:55:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36838d8cd4839ff406029e6bb1522cf44be6fbe6c7467921e5248b6c07a6aff5`  
		Last Modified: Wed, 10 Feb 2021 19:55:24 GMT  
		Size: 16.4 MB (16355614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e0f9d5139c635a9b975de4e63ad4f189516074a29dc56dd6d8fb7d277f433c`  
		Last Modified: Wed, 10 Feb 2021 19:55:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b851528d2df67a7c64ba6ffdffa9c9d295d9138c2118aa97ecb314bf8df40f31`  
		Last Modified: Wed, 10 Feb 2021 19:55:18 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abf701bca17610cfb13a04514ce3c1ae42cb17492484e2d3a1bce2a993a0f2f`  
		Last Modified: Wed, 10 Feb 2021 19:55:17 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f098af20d8519222d42bd836d1471d98ee831d2d922b13f7ca3c0b653c17f`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4267ee0ca74419bceecbf19e1465e0932bf90853f3268cfd144b6db60b8641`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f70a85d3b2f625c056ad12065547cd237ef4b5ae8a60449a5e85117837dcd4`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac9e58e231ffaac8a880d0de3eba5b4c2851b6a2a536719a3f3e45a660dd356`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d12c4db5395f443755c890788da47b44c0d59b25175fc18d1b0bcbca76f16c`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad520c9c3b5f0572b6c0ce26ef18a5ff0713f07f11a46974fd48597878e9da6`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef810b81f96651a0d2a0343fd3900d50c9f202fe114d740491fe64ea12c23815`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4c4b552633a82d1828c5cf24c2b3296792f992f6adae82c355822dbab99fd3`  
		Last Modified: Wed, 10 Feb 2021 19:55:13 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56267262030645aab5169f5cb94219ebbfe0427ab3d8f651e64956698f456`  
		Last Modified: Wed, 10 Feb 2021 19:55:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cfc4cbe95dd30bb06e52b3c2eaff805f74390d6241725fb431e28f21b0b988`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4e650a14400b1015308d7f542896c289c208edaa9b67dcc7c7c267290721cc`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d8f608756523415340070b95c5c66d516ab5ce49761a6d52f3c4bb374ceaab`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70036fc946d8c35838e5156a1cdbc4acfa0dfb7777e8a2b1c68c3575cabb773`  
		Last Modified: Wed, 10 Feb 2021 19:55:11 GMT  
		Size: 309.8 KB (309825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53eae9f2023fc3b9116bfae51eaad4e7a8eb05e67e9a03b8060a647e4cc47546`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:8f8fc4ea6e1563ee3ab2e75f793d715f62337829fa749303166f4c7b87b5fd6d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827259946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0764db061b485b056f35a9f55f331c66b513a6d4f5c94880eeb19647e3a07a6a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:44:53 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:46:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:46:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:46:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:46:17 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:46:18 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:46:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 10 Feb 2021 19:46:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:46:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:46:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:46:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:46:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:46:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:46:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:46:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:46:25 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:46:26 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:47:11 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:47:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0153fb9a550966fcb9a46155ee3f854d53cc8f5b93fd222e527469f624ed3864`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2428d9ebac128c1e235ea0193b3c686f3ac2ab39cab995e1c8950c8ba8337108`  
		Last Modified: Wed, 10 Feb 2021 19:55:52 GMT  
		Size: 21.8 MB (21775071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73e38964af26f07515595914dbb34cd08962428af69bf0f79a6c0acdb12df0`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2afd55956abba10688ff7bfcf894ee904de66d652a57b38f45d817ea24970f`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c40aa362fe3f06b3f8c638f3854b0003e87e83183e2d8255a4862257ec52aa5`  
		Last Modified: Wed, 10 Feb 2021 19:55:44 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cfeb85cad3ac53abec8be2a3433b84c7f3f596ea01b2bfd233a4d9604ddae5`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390c6e6af32e283bc45b0c07174103c4263221fa41133a3fb2e755338192a4db`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff06a60beba4f6825ecedb53f80e24c9c840cefc4a1e5d8e209caee2e93fd28e`  
		Last Modified: Wed, 10 Feb 2021 19:55:44 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761310cffade38a82d35d76a24350f795a0be62f747f960091dc6d74a9e42a4`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04119ba7d167513dc8fced1f79bd470007be8ea9e8cf3e7a61a57bdb2c9e437b`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcde858b06f73f425ae981873771bd224454ae0a366f3a03c03fa98c5866525d`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dcd0be1c9074d48807389fdb9bd95dd690cf6019fc42334d0a791b8a5a7941`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a62a5e70c867b79ba59a6ea275147b03ca5b486f341a045864fac3863beebb`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8878b460a7cfd33f71877a734283e4595adbd16400d59851fa802ce0a9a5d93`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b19f25838b5e2e96f5e8fe1bb366280f0c88b8fc1855eeb9b140a01c8ebc45`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1cabc58724baadec9cca0c08a3c1833f0179349372ce8115bf36021272f3f4`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b54c44ea72868954c9879ee9eefed550ba0bb56079307558f1c36b31f3147d`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb3bd379edf42c402d41f0d72f4ce290ff35087f1ff4d69d91c756fd113106c`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 267.8 KB (267828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5514ed308f579e66e3c855f9598400c11f48dfbd4719fd00c8ed95b852c8b9b9`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3d96451c1b2ead311a7713ebc9041a258403eef07611cce33cb5647b6b594909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:6da1bf1d8a609cef807ec4b7a3ad098a98655b240f92a1cedc0060c45c7bdb52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465382060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f096f4d4e87096ef9f385ee497d55a6e50fd022edf1d255d2dd3235578e1f18`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:42:31 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:42:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:43:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:43:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:43:01 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:43:02 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:43:02 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 10 Feb 2021 19:43:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:43:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:43:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:43:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:43:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:43:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:43:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:43:08 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:43:09 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:43:10 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:43:25 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:43:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfcfa417a148200a9b82e1221d8bf8897b6b076efa05274d844d5c53829055f`  
		Last Modified: Wed, 10 Feb 2021 19:55:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36838d8cd4839ff406029e6bb1522cf44be6fbe6c7467921e5248b6c07a6aff5`  
		Last Modified: Wed, 10 Feb 2021 19:55:24 GMT  
		Size: 16.4 MB (16355614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e0f9d5139c635a9b975de4e63ad4f189516074a29dc56dd6d8fb7d277f433c`  
		Last Modified: Wed, 10 Feb 2021 19:55:19 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b851528d2df67a7c64ba6ffdffa9c9d295d9138c2118aa97ecb314bf8df40f31`  
		Last Modified: Wed, 10 Feb 2021 19:55:18 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abf701bca17610cfb13a04514ce3c1ae42cb17492484e2d3a1bce2a993a0f2f`  
		Last Modified: Wed, 10 Feb 2021 19:55:17 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f098af20d8519222d42bd836d1471d98ee831d2d922b13f7ca3c0b653c17f`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4267ee0ca74419bceecbf19e1465e0932bf90853f3268cfd144b6db60b8641`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f70a85d3b2f625c056ad12065547cd237ef4b5ae8a60449a5e85117837dcd4`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac9e58e231ffaac8a880d0de3eba5b4c2851b6a2a536719a3f3e45a660dd356`  
		Last Modified: Wed, 10 Feb 2021 19:55:16 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d12c4db5395f443755c890788da47b44c0d59b25175fc18d1b0bcbca76f16c`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad520c9c3b5f0572b6c0ce26ef18a5ff0713f07f11a46974fd48597878e9da6`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef810b81f96651a0d2a0343fd3900d50c9f202fe114d740491fe64ea12c23815`  
		Last Modified: Wed, 10 Feb 2021 19:55:14 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4c4b552633a82d1828c5cf24c2b3296792f992f6adae82c355822dbab99fd3`  
		Last Modified: Wed, 10 Feb 2021 19:55:13 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56267262030645aab5169f5cb94219ebbfe0427ab3d8f651e64956698f456`  
		Last Modified: Wed, 10 Feb 2021 19:55:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cfc4cbe95dd30bb06e52b3c2eaff805f74390d6241725fb431e28f21b0b988`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4e650a14400b1015308d7f542896c289c208edaa9b67dcc7c7c267290721cc`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d8f608756523415340070b95c5c66d516ab5ce49761a6d52f3c4bb374ceaab`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70036fc946d8c35838e5156a1cdbc4acfa0dfb7777e8a2b1c68c3575cabb773`  
		Last Modified: Wed, 10 Feb 2021 19:55:11 GMT  
		Size: 309.8 KB (309825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53eae9f2023fc3b9116bfae51eaad4e7a8eb05e67e9a03b8060a647e4cc47546`  
		Last Modified: Wed, 10 Feb 2021 19:55:10 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:016c11e10a81c0e7f1f95e0270c9407ce10f51b919ce797fbb4d8fd08d9d7ca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:8f8fc4ea6e1563ee3ab2e75f793d715f62337829fa749303166f4c7b87b5fd6d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827259946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0764db061b485b056f35a9f55f331c66b513a6d4f5c94880eeb19647e3a07a6a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:44:53 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 10 Feb 2021 19:46:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:46:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:46:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:46:17 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:46:18 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:46:19 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 10 Feb 2021 19:46:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:46:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:46:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:46:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:46:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:46:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:46:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:46:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:46:25 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:46:26 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:47:11 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:47:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0153fb9a550966fcb9a46155ee3f854d53cc8f5b93fd222e527469f624ed3864`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2428d9ebac128c1e235ea0193b3c686f3ac2ab39cab995e1c8950c8ba8337108`  
		Last Modified: Wed, 10 Feb 2021 19:55:52 GMT  
		Size: 21.8 MB (21775071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73e38964af26f07515595914dbb34cd08962428af69bf0f79a6c0acdb12df0`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2afd55956abba10688ff7bfcf894ee904de66d652a57b38f45d817ea24970f`  
		Last Modified: Wed, 10 Feb 2021 19:55:46 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c40aa362fe3f06b3f8c638f3854b0003e87e83183e2d8255a4862257ec52aa5`  
		Last Modified: Wed, 10 Feb 2021 19:55:44 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cfeb85cad3ac53abec8be2a3433b84c7f3f596ea01b2bfd233a4d9604ddae5`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390c6e6af32e283bc45b0c07174103c4263221fa41133a3fb2e755338192a4db`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff06a60beba4f6825ecedb53f80e24c9c840cefc4a1e5d8e209caee2e93fd28e`  
		Last Modified: Wed, 10 Feb 2021 19:55:44 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761310cffade38a82d35d76a24350f795a0be62f747f960091dc6d74a9e42a4`  
		Last Modified: Wed, 10 Feb 2021 19:55:43 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04119ba7d167513dc8fced1f79bd470007be8ea9e8cf3e7a61a57bdb2c9e437b`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcde858b06f73f425ae981873771bd224454ae0a366f3a03c03fa98c5866525d`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dcd0be1c9074d48807389fdb9bd95dd690cf6019fc42334d0a791b8a5a7941`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a62a5e70c867b79ba59a6ea275147b03ca5b486f341a045864fac3863beebb`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8878b460a7cfd33f71877a734283e4595adbd16400d59851fa802ce0a9a5d93`  
		Last Modified: Wed, 10 Feb 2021 19:55:41 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b19f25838b5e2e96f5e8fe1bb366280f0c88b8fc1855eeb9b140a01c8ebc45`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1cabc58724baadec9cca0c08a3c1833f0179349372ce8115bf36021272f3f4`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b54c44ea72868954c9879ee9eefed550ba0bb56079307558f1c36b31f3147d`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb3bd379edf42c402d41f0d72f4ce290ff35087f1ff4d69d91c756fd113106c`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 267.8 KB (267828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5514ed308f579e66e3c855f9598400c11f48dfbd4719fd00c8ed95b852c8b9b9`  
		Last Modified: Wed, 10 Feb 2021 19:55:38 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:925100cc9e08c8d79ee37b36abe21d2f554982d5bf302c55a38f5da971f53431
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.3.0` - linux; amd64

```console
$ docker pull caddy@sha256:cbb1e84121ca20ac7fbc3cf8a9e04f4ee4979f33352ecfb883b56984fccf2cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73dc9258a8ebf0244d67701a655c1fc655cbfda642ab615e06b1a6039d5b2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:19:40 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:19:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:19:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:19:43 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:46 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe9aaa681bd550de2455df437d9c9a9e24005e810e7d5a01c35d263fa2aa46`  
		Last Modified: Mon, 04 Jan 2021 18:20:23 GMT  
		Size: 11.6 MB (11622354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3b11169846dc2fcfacfbcaae13fcc50c8b72dc70b6bc9c4cfd9f156a37c4c`  
		Last Modified: Mon, 04 Jan 2021 18:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b11903d75dc786cc7a333dcc8eb86432e12286a27596ba9a13de8ce6a16bbe4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f2d0ff6672d884939bbd0e7ae29c28c4a54054bfb0132b16a6fd7144ccf4d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:49:38 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:49:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:49:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:49:46 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:49:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:49:51 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:49:53 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:49:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493ce1c2e0e02619db2817c3da32453658bbca2b087c8d73cf9c8eae72e5926`  
		Last Modified: Mon, 04 Jan 2021 18:50:38 GMT  
		Size: 10.9 MB (10944839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a640f55dfe60d817bb1c48cf163e52c3c42b843b7aa9976d573ac5b4bb322a04`  
		Last Modified: Mon, 04 Jan 2021 18:50:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8d7dd8d7f22f669d44669e643d61092c90ec7c1bcd4704e119d72715dc4b7de1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8ff470d547b26a0bf496261541723024fa700eb9d162dad5eba091a1320ce5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:57:42 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:57:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:57:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:57:49 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:57:49 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:57:50 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:57:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:57:57 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:57:58 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1178be4a6bd4aee0a16e25358732f4deac6a84f6614bd4d5a9d242ac9068d`  
		Last Modified: Mon, 04 Jan 2021 18:58:43 GMT  
		Size: 10.9 MB (10925337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb438ac85eaa28804b9de2f3e230fe52916ba5b81a38b03c514f2dbe9282c679`  
		Last Modified: Mon, 04 Jan 2021 18:58:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93f5ca2902036950ab4ab8a22f4d74f36bce55feee9b7e0e797396e2d07f4df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9774262cda02b94b5c9cc6bfc57d947819c3a0f1e85aacb278c6e91ddd7850`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:39:58 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:40:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:40:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:40:03 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:40:04 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:40:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:40:17 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:40:18 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:40:19 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:40:19 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48312421be65c130b3524264024f10c7774e9eab1b9cf370a6c7022753927567`  
		Last Modified: Mon, 04 Jan 2021 18:41:12 GMT  
		Size: 10.6 MB (10598984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332c70787e2588f66eeb0b6abd933d1f004e4f0357a5618092fdb36f9e88913f`  
		Last Modified: Mon, 04 Jan 2021 18:41:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:1be56543a90159f9a8bd5a83094c762bda8baef783604503316fcafbc5467c09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13354933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b014a3125a542b761c87a24c6c1c5f71f964b4414c310af9ce20822717a8e2ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:17:34 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:18:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:18:12 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:18:18 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:18:23 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:18:29 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:18:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:27 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:43 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:50 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:55 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecaad708cba83777a49b8b0153fd11aa1fda8c3de8c2669359510c7fba8e1d4`  
		Last Modified: Mon, 04 Jan 2021 18:21:19 GMT  
		Size: 10.2 MB (10241384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235fec692a51bccc1545ea1f8f892604e9198ae61248e12ddeba4043bea2c1f3`  
		Last Modified: Mon, 04 Jan 2021 18:21:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; s390x

```console
$ docker pull caddy@sha256:1d605f274d1eca015a6899f98aed7e87ddbcf21fee25db45eb3af04b7fa35c7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a2f900066e27e26138f6cac769b05f6cd3b0c6859052c1aa39eba8665d1a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:41:41 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:41:47 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:41:48 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e914cfc82e9092a831f17f5daebbbde8ebe39d7fe50230325ce80f657bfe3f0f`  
		Last Modified: Mon, 04 Jan 2021 18:42:29 GMT  
		Size: 11.3 MB (11272057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d554de8138d32421dfdcb23f0feec824f7106586791ae523f39943c710ad71`  
		Last Modified: Mon, 04 Jan 2021 18:42:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-alpine`

```console
$ docker pull caddy@sha256:99d811b358ec3f3bc45a430c6358fc7af75423cb047012518fdd1708f5b2dc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.3.0-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:cbb1e84121ca20ac7fbc3cf8a9e04f4ee4979f33352ecfb883b56984fccf2cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73dc9258a8ebf0244d67701a655c1fc655cbfda642ab615e06b1a6039d5b2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:19:40 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:19:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:19:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:19:43 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:46 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe9aaa681bd550de2455df437d9c9a9e24005e810e7d5a01c35d263fa2aa46`  
		Last Modified: Mon, 04 Jan 2021 18:20:23 GMT  
		Size: 11.6 MB (11622354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3b11169846dc2fcfacfbcaae13fcc50c8b72dc70b6bc9c4cfd9f156a37c4c`  
		Last Modified: Mon, 04 Jan 2021 18:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b11903d75dc786cc7a333dcc8eb86432e12286a27596ba9a13de8ce6a16bbe4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f2d0ff6672d884939bbd0e7ae29c28c4a54054bfb0132b16a6fd7144ccf4d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:49:38 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:49:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:49:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:49:46 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:49:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:49:51 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:49:53 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:49:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493ce1c2e0e02619db2817c3da32453658bbca2b087c8d73cf9c8eae72e5926`  
		Last Modified: Mon, 04 Jan 2021 18:50:38 GMT  
		Size: 10.9 MB (10944839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a640f55dfe60d817bb1c48cf163e52c3c42b843b7aa9976d573ac5b4bb322a04`  
		Last Modified: Mon, 04 Jan 2021 18:50:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8d7dd8d7f22f669d44669e643d61092c90ec7c1bcd4704e119d72715dc4b7de1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8ff470d547b26a0bf496261541723024fa700eb9d162dad5eba091a1320ce5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:57:42 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:57:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:57:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:57:49 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:57:49 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:57:50 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:57:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:57:57 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:57:58 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1178be4a6bd4aee0a16e25358732f4deac6a84f6614bd4d5a9d242ac9068d`  
		Last Modified: Mon, 04 Jan 2021 18:58:43 GMT  
		Size: 10.9 MB (10925337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb438ac85eaa28804b9de2f3e230fe52916ba5b81a38b03c514f2dbe9282c679`  
		Last Modified: Mon, 04 Jan 2021 18:58:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93f5ca2902036950ab4ab8a22f4d74f36bce55feee9b7e0e797396e2d07f4df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9774262cda02b94b5c9cc6bfc57d947819c3a0f1e85aacb278c6e91ddd7850`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:39:58 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:40:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:40:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:40:03 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:40:04 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:40:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:40:17 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:40:18 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:40:19 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:40:19 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48312421be65c130b3524264024f10c7774e9eab1b9cf370a6c7022753927567`  
		Last Modified: Mon, 04 Jan 2021 18:41:12 GMT  
		Size: 10.6 MB (10598984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332c70787e2588f66eeb0b6abd933d1f004e4f0357a5618092fdb36f9e88913f`  
		Last Modified: Mon, 04 Jan 2021 18:41:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1be56543a90159f9a8bd5a83094c762bda8baef783604503316fcafbc5467c09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13354933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b014a3125a542b761c87a24c6c1c5f71f964b4414c310af9ce20822717a8e2ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:17:34 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:18:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:18:12 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:18:18 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:18:23 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:18:29 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:18:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:27 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:43 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:50 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:55 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecaad708cba83777a49b8b0153fd11aa1fda8c3de8c2669359510c7fba8e1d4`  
		Last Modified: Mon, 04 Jan 2021 18:21:19 GMT  
		Size: 10.2 MB (10241384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235fec692a51bccc1545ea1f8f892604e9198ae61248e12ddeba4043bea2c1f3`  
		Last Modified: Mon, 04 Jan 2021 18:21:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1d605f274d1eca015a6899f98aed7e87ddbcf21fee25db45eb3af04b7fa35c7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a2f900066e27e26138f6cac769b05f6cd3b0c6859052c1aa39eba8665d1a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:41:41 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:41:47 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:41:48 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e914cfc82e9092a831f17f5daebbbde8ebe39d7fe50230325ce80f657bfe3f0f`  
		Last Modified: Mon, 04 Jan 2021 18:42:29 GMT  
		Size: 11.3 MB (11272057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d554de8138d32421dfdcb23f0feec824f7106586791ae523f39943c710ad71`  
		Last Modified: Mon, 04 Jan 2021 18:42:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder`

```console
$ docker pull caddy@sha256:763a7e82924f2c442cc5a3d3d1d41387f63b52a51382c106e8439ce507f36586
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.3.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:d5bb32fa0e3f9a239adaa5ac70cebf0e03a3e346ea4d868b13d58557008deca4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991340368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11eaab85c697a5c8abc66041176b8fdbf82fdf94f646a817c0a50cb11b4bea5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:53:10 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:53:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:54:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:54:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f750d5f99c1a9ce469b75988e116b0eba426108f651529f6e3757c5d51d8052`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099199a322708ecb52e115f11a625afe3e6015cdd0ee214d383383499a0762c2`  
		Last Modified: Wed, 10 Feb 2021 19:57:46 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c8ee528f7c43df3b8920a572b361f8fbea5010461aac26d1be73fe8c82236`  
		Last Modified: Wed, 10 Feb 2021 19:58:00 GMT  
		Size: 11.5 MB (11509432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b46752396f341b0ec6bb7e56ac9e7a2b139e2c981013c1d0552b70b027d1`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:9f2442e39180a6b96658075c5ff728c664269c7bbfc27b27d937ec4acdb5d6bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.3.0-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c945eeb5d1d62d1b05b7f0ec48c00bf6e000b0cf9c3473664ebcee6988c8326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:61f14aae2331d3e79e2ba08babbd5d99f96285dfc0d27cd73efddd68bd4f0c39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:d5bb32fa0e3f9a239adaa5ac70cebf0e03a3e346ea4d868b13d58557008deca4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991340368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11eaab85c697a5c8abc66041176b8fdbf82fdf94f646a817c0a50cb11b4bea5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:53:10 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:53:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:54:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:54:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f750d5f99c1a9ce469b75988e116b0eba426108f651529f6e3757c5d51d8052`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099199a322708ecb52e115f11a625afe3e6015cdd0ee214d383383499a0762c2`  
		Last Modified: Wed, 10 Feb 2021 19:57:46 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c8ee528f7c43df3b8920a572b361f8fbea5010461aac26d1be73fe8c82236`  
		Last Modified: Wed, 10 Feb 2021 19:58:00 GMT  
		Size: 11.5 MB (11509432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b46752396f341b0ec6bb7e56ac9e7a2b139e2c981013c1d0552b70b027d1`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore`

```console
$ docker pull caddy@sha256:7e6d94f3b7aacaa4e3b30c830fa5ac3faf4c439d296e297ff096b819703c3626
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.3.0-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c79b179601df4a576d0db9f8794e73dd656a5cb1f19dee2ea92785f7a26f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.3.0-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:01472e271cb930e4158b91691b2b0c8b03ae719bd9cd00cbf5244e41bde54d9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:99d811b358ec3f3bc45a430c6358fc7af75423cb047012518fdd1708f5b2dc71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:cbb1e84121ca20ac7fbc3cf8a9e04f4ee4979f33352ecfb883b56984fccf2cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73dc9258a8ebf0244d67701a655c1fc655cbfda642ab615e06b1a6039d5b2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:19:40 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:19:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:19:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:19:43 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:46 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe9aaa681bd550de2455df437d9c9a9e24005e810e7d5a01c35d263fa2aa46`  
		Last Modified: Mon, 04 Jan 2021 18:20:23 GMT  
		Size: 11.6 MB (11622354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3b11169846dc2fcfacfbcaae13fcc50c8b72dc70b6bc9c4cfd9f156a37c4c`  
		Last Modified: Mon, 04 Jan 2021 18:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b11903d75dc786cc7a333dcc8eb86432e12286a27596ba9a13de8ce6a16bbe4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f2d0ff6672d884939bbd0e7ae29c28c4a54054bfb0132b16a6fd7144ccf4d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:49:38 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:49:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:49:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:49:46 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:49:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:49:51 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:49:53 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:49:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493ce1c2e0e02619db2817c3da32453658bbca2b087c8d73cf9c8eae72e5926`  
		Last Modified: Mon, 04 Jan 2021 18:50:38 GMT  
		Size: 10.9 MB (10944839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a640f55dfe60d817bb1c48cf163e52c3c42b843b7aa9976d573ac5b4bb322a04`  
		Last Modified: Mon, 04 Jan 2021 18:50:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8d7dd8d7f22f669d44669e643d61092c90ec7c1bcd4704e119d72715dc4b7de1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8ff470d547b26a0bf496261541723024fa700eb9d162dad5eba091a1320ce5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:57:42 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:57:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:57:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:57:49 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:57:49 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:57:50 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:57:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:57:57 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:57:58 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1178be4a6bd4aee0a16e25358732f4deac6a84f6614bd4d5a9d242ac9068d`  
		Last Modified: Mon, 04 Jan 2021 18:58:43 GMT  
		Size: 10.9 MB (10925337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb438ac85eaa28804b9de2f3e230fe52916ba5b81a38b03c514f2dbe9282c679`  
		Last Modified: Mon, 04 Jan 2021 18:58:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93f5ca2902036950ab4ab8a22f4d74f36bce55feee9b7e0e797396e2d07f4df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9774262cda02b94b5c9cc6bfc57d947819c3a0f1e85aacb278c6e91ddd7850`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:39:58 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:40:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:40:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:40:03 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:40:04 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:40:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:40:17 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:40:18 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:40:19 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:40:19 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48312421be65c130b3524264024f10c7774e9eab1b9cf370a6c7022753927567`  
		Last Modified: Mon, 04 Jan 2021 18:41:12 GMT  
		Size: 10.6 MB (10598984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332c70787e2588f66eeb0b6abd933d1f004e4f0357a5618092fdb36f9e88913f`  
		Last Modified: Mon, 04 Jan 2021 18:41:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1be56543a90159f9a8bd5a83094c762bda8baef783604503316fcafbc5467c09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13354933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b014a3125a542b761c87a24c6c1c5f71f964b4414c310af9ce20822717a8e2ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:17:34 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:18:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:18:12 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:18:18 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:18:23 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:18:29 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:18:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:27 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:43 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:50 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:55 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecaad708cba83777a49b8b0153fd11aa1fda8c3de8c2669359510c7fba8e1d4`  
		Last Modified: Mon, 04 Jan 2021 18:21:19 GMT  
		Size: 10.2 MB (10241384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235fec692a51bccc1545ea1f8f892604e9198ae61248e12ddeba4043bea2c1f3`  
		Last Modified: Mon, 04 Jan 2021 18:21:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1d605f274d1eca015a6899f98aed7e87ddbcf21fee25db45eb3af04b7fa35c7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a2f900066e27e26138f6cac769b05f6cd3b0c6859052c1aa39eba8665d1a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:41:41 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:41:47 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:41:48 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e914cfc82e9092a831f17f5daebbbde8ebe39d7fe50230325ce80f657bfe3f0f`  
		Last Modified: Mon, 04 Jan 2021 18:42:29 GMT  
		Size: 11.3 MB (11272057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d554de8138d32421dfdcb23f0feec824f7106586791ae523f39943c710ad71`  
		Last Modified: Mon, 04 Jan 2021 18:42:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:763a7e82924f2c442cc5a3d3d1d41387f63b52a51382c106e8439ce507f36586
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:d5bb32fa0e3f9a239adaa5ac70cebf0e03a3e346ea4d868b13d58557008deca4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991340368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11eaab85c697a5c8abc66041176b8fdbf82fdf94f646a817c0a50cb11b4bea5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:53:10 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:53:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:54:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:54:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f750d5f99c1a9ce469b75988e116b0eba426108f651529f6e3757c5d51d8052`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099199a322708ecb52e115f11a625afe3e6015cdd0ee214d383383499a0762c2`  
		Last Modified: Wed, 10 Feb 2021 19:57:46 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c8ee528f7c43df3b8920a572b361f8fbea5010461aac26d1be73fe8c82236`  
		Last Modified: Wed, 10 Feb 2021 19:58:00 GMT  
		Size: 11.5 MB (11509432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b46752396f341b0ec6bb7e56ac9e7a2b139e2c981013c1d0552b70b027d1`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:9f2442e39180a6b96658075c5ff728c664269c7bbfc27b27d937ec4acdb5d6bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c945eeb5d1d62d1b05b7f0ec48c00bf6e000b0cf9c3473664ebcee6988c8326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:61f14aae2331d3e79e2ba08babbd5d99f96285dfc0d27cd73efddd68bd4f0c39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:d5bb32fa0e3f9a239adaa5ac70cebf0e03a3e346ea4d868b13d58557008deca4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991340368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11eaab85c697a5c8abc66041176b8fdbf82fdf94f646a817c0a50cb11b4bea5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:53:10 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:53:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:54:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:54:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f750d5f99c1a9ce469b75988e116b0eba426108f651529f6e3757c5d51d8052`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099199a322708ecb52e115f11a625afe3e6015cdd0ee214d383383499a0762c2`  
		Last Modified: Wed, 10 Feb 2021 19:57:46 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c8ee528f7c43df3b8920a572b361f8fbea5010461aac26d1be73fe8c82236`  
		Last Modified: Wed, 10 Feb 2021 19:58:00 GMT  
		Size: 11.5 MB (11509432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b46752396f341b0ec6bb7e56ac9e7a2b139e2c981013c1d0552b70b027d1`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:7e6d94f3b7aacaa4e3b30c830fa5ac3faf4c439d296e297ff096b819703c3626
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c79b179601df4a576d0db9f8794e73dd656a5cb1f19dee2ea92785f7a26f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:01472e271cb930e4158b91691b2b0c8b03ae719bd9cd00cbf5244e41bde54d9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:99d811b358ec3f3bc45a430c6358fc7af75423cb047012518fdd1708f5b2dc71
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
$ docker pull caddy@sha256:cbb1e84121ca20ac7fbc3cf8a9e04f4ee4979f33352ecfb883b56984fccf2cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73dc9258a8ebf0244d67701a655c1fc655cbfda642ab615e06b1a6039d5b2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:19:40 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:19:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:19:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:19:43 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:46 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe9aaa681bd550de2455df437d9c9a9e24005e810e7d5a01c35d263fa2aa46`  
		Last Modified: Mon, 04 Jan 2021 18:20:23 GMT  
		Size: 11.6 MB (11622354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3b11169846dc2fcfacfbcaae13fcc50c8b72dc70b6bc9c4cfd9f156a37c4c`  
		Last Modified: Mon, 04 Jan 2021 18:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b11903d75dc786cc7a333dcc8eb86432e12286a27596ba9a13de8ce6a16bbe4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f2d0ff6672d884939bbd0e7ae29c28c4a54054bfb0132b16a6fd7144ccf4d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:49:38 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:49:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:49:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:49:46 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:49:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:49:51 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:49:53 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:49:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493ce1c2e0e02619db2817c3da32453658bbca2b087c8d73cf9c8eae72e5926`  
		Last Modified: Mon, 04 Jan 2021 18:50:38 GMT  
		Size: 10.9 MB (10944839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a640f55dfe60d817bb1c48cf163e52c3c42b843b7aa9976d573ac5b4bb322a04`  
		Last Modified: Mon, 04 Jan 2021 18:50:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8d7dd8d7f22f669d44669e643d61092c90ec7c1bcd4704e119d72715dc4b7de1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8ff470d547b26a0bf496261541723024fa700eb9d162dad5eba091a1320ce5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:57:42 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:57:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:57:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:57:49 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:57:49 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:57:50 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:57:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:57:57 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:57:58 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1178be4a6bd4aee0a16e25358732f4deac6a84f6614bd4d5a9d242ac9068d`  
		Last Modified: Mon, 04 Jan 2021 18:58:43 GMT  
		Size: 10.9 MB (10925337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb438ac85eaa28804b9de2f3e230fe52916ba5b81a38b03c514f2dbe9282c679`  
		Last Modified: Mon, 04 Jan 2021 18:58:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93f5ca2902036950ab4ab8a22f4d74f36bce55feee9b7e0e797396e2d07f4df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9774262cda02b94b5c9cc6bfc57d947819c3a0f1e85aacb278c6e91ddd7850`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:39:58 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:40:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:40:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:40:03 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:40:04 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:40:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:40:17 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:40:18 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:40:19 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:40:19 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48312421be65c130b3524264024f10c7774e9eab1b9cf370a6c7022753927567`  
		Last Modified: Mon, 04 Jan 2021 18:41:12 GMT  
		Size: 10.6 MB (10598984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332c70787e2588f66eeb0b6abd933d1f004e4f0357a5618092fdb36f9e88913f`  
		Last Modified: Mon, 04 Jan 2021 18:41:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1be56543a90159f9a8bd5a83094c762bda8baef783604503316fcafbc5467c09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13354933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b014a3125a542b761c87a24c6c1c5f71f964b4414c310af9ce20822717a8e2ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:17:34 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:18:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:18:12 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:18:18 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:18:23 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:18:29 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:18:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:27 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:43 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:50 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:55 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecaad708cba83777a49b8b0153fd11aa1fda8c3de8c2669359510c7fba8e1d4`  
		Last Modified: Mon, 04 Jan 2021 18:21:19 GMT  
		Size: 10.2 MB (10241384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235fec692a51bccc1545ea1f8f892604e9198ae61248e12ddeba4043bea2c1f3`  
		Last Modified: Mon, 04 Jan 2021 18:21:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1d605f274d1eca015a6899f98aed7e87ddbcf21fee25db45eb3af04b7fa35c7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a2f900066e27e26138f6cac769b05f6cd3b0c6859052c1aa39eba8665d1a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:41:41 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:41:47 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:41:48 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e914cfc82e9092a831f17f5daebbbde8ebe39d7fe50230325ce80f657bfe3f0f`  
		Last Modified: Mon, 04 Jan 2021 18:42:29 GMT  
		Size: 11.3 MB (11272057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d554de8138d32421dfdcb23f0feec824f7106586791ae523f39943c710ad71`  
		Last Modified: Mon, 04 Jan 2021 18:42:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:763a7e82924f2c442cc5a3d3d1d41387f63b52a51382c106e8439ce507f36586
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:d5bb32fa0e3f9a239adaa5ac70cebf0e03a3e346ea4d868b13d58557008deca4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991340368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11eaab85c697a5c8abc66041176b8fdbf82fdf94f646a817c0a50cb11b4bea5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:53:10 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:53:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:54:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:54:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f750d5f99c1a9ce469b75988e116b0eba426108f651529f6e3757c5d51d8052`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099199a322708ecb52e115f11a625afe3e6015cdd0ee214d383383499a0762c2`  
		Last Modified: Wed, 10 Feb 2021 19:57:46 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c8ee528f7c43df3b8920a572b361f8fbea5010461aac26d1be73fe8c82236`  
		Last Modified: Wed, 10 Feb 2021 19:58:00 GMT  
		Size: 11.5 MB (11509432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b46752396f341b0ec6bb7e56ac9e7a2b139e2c981013c1d0552b70b027d1`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:9f2442e39180a6b96658075c5ff728c664269c7bbfc27b27d937ec4acdb5d6bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c945eeb5d1d62d1b05b7f0ec48c00bf6e000b0cf9c3473664ebcee6988c8326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:61f14aae2331d3e79e2ba08babbd5d99f96285dfc0d27cd73efddd68bd4f0c39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:d5bb32fa0e3f9a239adaa5ac70cebf0e03a3e346ea4d868b13d58557008deca4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991340368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11eaab85c697a5c8abc66041176b8fdbf82fdf94f646a817c0a50cb11b4bea5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:53:10 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:53:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:54:29 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:54:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac440c2f3dca4d40aa0fe9622792b1e29a0881e677ef7f234a0c7c65c202f7a`  
		Last Modified: Wed, 10 Feb 2021 19:56:20 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f750d5f99c1a9ce469b75988e116b0eba426108f651529f6e3757c5d51d8052`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099199a322708ecb52e115f11a625afe3e6015cdd0ee214d383383499a0762c2`  
		Last Modified: Wed, 10 Feb 2021 19:57:46 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c8ee528f7c43df3b8920a572b361f8fbea5010461aac26d1be73fe8c82236`  
		Last Modified: Wed, 10 Feb 2021 19:58:00 GMT  
		Size: 11.5 MB (11509432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b46752396f341b0ec6bb7e56ac9e7a2b139e2c981013c1d0552b70b027d1`  
		Last Modified: Wed, 10 Feb 2021 19:57:45 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:925100cc9e08c8d79ee37b36abe21d2f554982d5bf302c55a38f5da971f53431
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:cbb1e84121ca20ac7fbc3cf8a9e04f4ee4979f33352ecfb883b56984fccf2cd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73dc9258a8ebf0244d67701a655c1fc655cbfda642ab615e06b1a6039d5b2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:34:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 12:35:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:19:40 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:19:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:19:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:19:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:19:43 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:19:43 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:19:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:45 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:46 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afadb5ee6ea5f6d507d8b77b8ba0ace43c1db0a163815f209e62439af325d6c`  
		Last Modified: Thu, 17 Dec 2020 12:36:36 GMT  
		Size: 300.0 KB (299951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e5593f16cf4f0a44a49cdf9021457e530ba060d4610405b1d37004ab643d79`  
		Last Modified: Thu, 17 Dec 2020 12:36:45 GMT  
		Size: 5.8 KB (5758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe9aaa681bd550de2455df437d9c9a9e24005e810e7d5a01c35d263fa2aa46`  
		Last Modified: Mon, 04 Jan 2021 18:20:23 GMT  
		Size: 11.6 MB (11622354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f3b11169846dc2fcfacfbcaae13fcc50c8b72dc70b6bc9c4cfd9f156a37c4c`  
		Last Modified: Mon, 04 Jan 2021 18:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b11903d75dc786cc7a333dcc8eb86432e12286a27596ba9a13de8ce6a16bbe4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f2d0ff6672d884939bbd0e7ae29c28c4a54054bfb0132b16a6fd7144ccf4d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:57:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:58:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:49:38 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:49:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:49:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:49:46 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:49:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:49:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:49:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:49:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:49:51 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:49:52 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:49:53 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:49:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab316ae645fb129ec71432847f46832070abbd380444d7a049031cbef03c39`  
		Last Modified: Thu, 17 Dec 2020 00:59:38 GMT  
		Size: 300.1 KB (300099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c408732dcfb31f73b6a82942aa3e9ab50640eaeb49c175dcfddab4b07f0e790`  
		Last Modified: Thu, 17 Dec 2020 00:59:51 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7493ce1c2e0e02619db2817c3da32453658bbca2b087c8d73cf9c8eae72e5926`  
		Last Modified: Mon, 04 Jan 2021 18:50:38 GMT  
		Size: 10.9 MB (10944839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a640f55dfe60d817bb1c48cf163e52c3c42b843b7aa9976d573ac5b4bb322a04`  
		Last Modified: Mon, 04 Jan 2021 18:50:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8d7dd8d7f22f669d44669e643d61092c90ec7c1bcd4704e119d72715dc4b7de1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8ff470d547b26a0bf496261541723024fa700eb9d162dad5eba091a1320ce5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:02:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 01:02:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:57:42 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:57:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:57:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:57:49 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:57:49 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:57:50 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:57:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:57:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:57:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:57:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:57:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:57:56 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:57:57 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:57:58 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409aee3f1c32dd7aeea094975a27bd66a5c78389115618ff162028b950dd4b2`  
		Last Modified: Thu, 17 Dec 2020 01:04:59 GMT  
		Size: 299.2 KB (299192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d150f546c9b585983f5e6390aa4e292e940deda5ca6eafab23f7eccd86e1f`  
		Last Modified: Thu, 17 Dec 2020 01:05:12 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1178be4a6bd4aee0a16e25358732f4deac6a84f6614bd4d5a9d242ac9068d`  
		Last Modified: Mon, 04 Jan 2021 18:58:43 GMT  
		Size: 10.9 MB (10925337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb438ac85eaa28804b9de2f3e230fe52916ba5b81a38b03c514f2dbe9282c679`  
		Last Modified: Mon, 04 Jan 2021 18:58:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:93f5ca2902036950ab4ab8a22f4d74f36bce55feee9b7e0e797396e2d07f4df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9774262cda02b94b5c9cc6bfc57d947819c3a0f1e85aacb278c6e91ddd7850`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:32:45 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:33:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:39:58 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:40:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:40:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:40:03 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:40:04 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:40:05 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:40:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:40:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:40:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:40:17 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:40:18 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:40:19 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:40:19 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6b1f8553a8382b04fce0860980a988a45e1e4efa692cd394306560d4d8352`  
		Last Modified: Thu, 17 Dec 2020 00:35:31 GMT  
		Size: 300.3 KB (300344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e695d7a94fe7f9e9c0dd063d219b5498420a85648620408166c2eba6a1fc81f`  
		Last Modified: Thu, 17 Dec 2020 00:35:41 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48312421be65c130b3524264024f10c7774e9eab1b9cf370a6c7022753927567`  
		Last Modified: Mon, 04 Jan 2021 18:41:12 GMT  
		Size: 10.6 MB (10598984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332c70787e2588f66eeb0b6abd933d1f004e4f0357a5618092fdb36f9e88913f`  
		Last Modified: Mon, 04 Jan 2021 18:41:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:1be56543a90159f9a8bd5a83094c762bda8baef783604503316fcafbc5467c09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13354933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b014a3125a542b761c87a24c6c1c5f71f964b4414c310af9ce20822717a8e2ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 02:29:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:17:34 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:18:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:18:12 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:18:18 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:18:23 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:18:29 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:18:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:19:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:19:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:19:27 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:19:43 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:19:50 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:19:55 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:19:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5661232cea07dc41ae167e15c374f79251b26170652b994e8844fb55b4a5410`  
		Last Modified: Thu, 17 Dec 2020 02:34:34 GMT  
		Size: 302.3 KB (302338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6c5134cf53417dab24ffba916fe2c36f64c91f8109cd4035ce97e9d2efa6f`  
		Last Modified: Thu, 17 Dec 2020 02:34:48 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecaad708cba83777a49b8b0153fd11aa1fda8c3de8c2669359510c7fba8e1d4`  
		Last Modified: Mon, 04 Jan 2021 18:21:19 GMT  
		Size: 10.2 MB (10241384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235fec692a51bccc1545ea1f8f892604e9198ae61248e12ddeba4043bea2c1f3`  
		Last Modified: Mon, 04 Jan 2021 18:21:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:1d605f274d1eca015a6899f98aed7e87ddbcf21fee25db45eb3af04b7fa35c7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a2f900066e27e26138f6cac769b05f6cd3b0c6859052c1aa39eba8665d1a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 17 Dec 2020 00:26:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Mon, 04 Jan 2021 18:41:41 GMT
ENV CADDY_VERSION=v2.3.0
# Mon, 04 Jan 2021 18:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 Jan 2021 18:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 Jan 2021 18:41:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/config]
# Mon, 04 Jan 2021 18:41:45 GMT
VOLUME [/data]
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 Jan 2021 18:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 Jan 2021 18:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 Jan 2021 18:41:47 GMT
EXPOSE 80
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 443
# Mon, 04 Jan 2021 18:41:48 GMT
EXPOSE 2019
# Mon, 04 Jan 2021 18:41:48 GMT
WORKDIR /srv
# Mon, 04 Jan 2021 18:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540682837d130d7c39e8c04e25653ea251d395459d10b412bfe6ef4350bf64e4`  
		Last Modified: Thu, 17 Dec 2020 00:28:06 GMT  
		Size: 300.5 KB (300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cd745d1483c5464a545008c053bd17567c01d9e53779365080e1ac3d4207da`  
		Last Modified: Thu, 17 Dec 2020 00:28:17 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e914cfc82e9092a831f17f5daebbbde8ebe39d7fe50230325ce80f657bfe3f0f`  
		Last Modified: Mon, 04 Jan 2021 18:42:29 GMT  
		Size: 11.3 MB (11272057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d554de8138d32421dfdcb23f0feec824f7106586791ae523f39943c710ad71`  
		Last Modified: Mon, 04 Jan 2021 18:42:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:7e6d94f3b7aacaa4e3b30c830fa5ac3faf4c439d296e297ff096b819703c3626
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c79b179601df4a576d0db9f8794e73dd656a5cb1f19dee2ea92785f7a26f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:7cc10fb87e454eb5d441260303aa26c2811ef94a2ab1d8943868bd27764b2b4d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bb21c950d8f98025db92e5d6f4672ef8245fedbc946ff983d23420a93d25b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:42:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:49:12 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:49:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:49:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:49:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:49:41 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:49:42 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:49:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:49:48 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:49:49 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:50:03 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:50:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc999509f6ae39fd1c7356e8f8ab048d5fccd9046895a2985d08041dfdbee5b`  
		Last Modified: Wed, 10 Feb 2021 19:55:30 GMT  
		Size: 9.4 MB (9425439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2625f1138b8161c8b9470637b7d998f92d78ab822c0169656e29cc2d53db41f`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820193dcc2b627f60af839975e0b6c0bcf8a267043f4c21518c70763e3bedf5`  
		Last Modified: Wed, 10 Feb 2021 19:56:45 GMT  
		Size: 16.4 MB (16437306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874858411ee2482c1868893e51f31a074f503f89f80f058e048658ebe30d9246`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd13d8d5005d3c598a9988de4e8c318e23ad11b73f5ba2d6d17f2c0a8f6112`  
		Last Modified: Wed, 10 Feb 2021 19:56:41 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14797008a1e95ea4f4feb6690d3eb858f9af4ff3c29e5c951340114f5103c5`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476f1a710388b0ae374ab33f473abbc5fcbdde056584c61b42274f6afd93246`  
		Last Modified: Wed, 10 Feb 2021 19:56:39 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f754e6d8d4cb78c42eb93d60919640bb018d4eab1e1d98dc81f5e784e2054c`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522d5f845b9bc74b139ddf41dd2412e5b0f98ad74a200908757dbb98223ad10`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442db462ebe51ef1447f85f3ff7fcde8702e733f8fc441ddead5b37ad9eaf590`  
		Last Modified: Wed, 10 Feb 2021 19:56:38 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219654456f23077b35a20a3a49821bb83aa248e9985257d1b544eff576dc642`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42bb7e5f7594b12e74c58cdf7ec06fd58b33624c319e770c0e948078b98bb4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557776033ee5573096bdb1bba3bbe59273b65e5541ee2c743016d49101c9d0d8`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c9a36915b169435045b40d252c8df5aae311fb08bc38e4fe9919d3a64e92a4`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f532ce47654a29125b0b66c168e8a85ed7f8eda5787037d5fb9d34f1c9037861`  
		Last Modified: Wed, 10 Feb 2021 19:56:36 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f333f658558cc9efa81a790cfcc4c32aa577b3554fb88ec46d97edb8babb88`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b0d95eb155b38dece1e992d9b147065abc461ebdc7369351c19af7a7802b9`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac09a5d17783f9f917c0c6517c4f0f186fd742ad8e3d047badee7480446eae4`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b05d79e7981565e4b174dcd4fea2098eb2dd8cbcd6681710e2cd14af95e36`  
		Last Modified: Wed, 10 Feb 2021 19:56:34 GMT  
		Size: 298.0 KB (297966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b45069483243ed9fe4c38ab5f9710624d0aedd62dd181b3fa8a2c70dfefe76`  
		Last Modified: Wed, 10 Feb 2021 19:56:33 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:01472e271cb930e4158b91691b2b0c8b03ae719bd9cd00cbf5244e41bde54d9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
