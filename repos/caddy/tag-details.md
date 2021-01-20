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
$ docker pull caddy@sha256:089eb574cd5464872ede3cd6adb1e12eee92c6f43355794b74438c671ffee975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

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

### `caddy:2` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1`

```console
$ docker pull caddy@sha256:8e258a4ca3a881f0ac013f5617b82a04a69433381d88980c8d2f46cec42ef8ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

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

### `caddy:2.2.1` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:d609c829f7d4a0747c339fe7dc0f43c53dc981c5c5c974aea1897eed3ac7f971
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461757069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62e3aa62d54d82435bcaf541e63ef826fbb38a40c1a7db894d5fe37948c3d14`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Jan 2021 23:55:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 13 Jan 2021 23:55:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Jan 2021 23:55:37 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Jan 2021 23:55:38 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Jan 2021 23:55:39 GMT
VOLUME [c:/config]
# Wed, 13 Jan 2021 23:55:39 GMT
VOLUME [c:/data]
# Wed, 13 Jan 2021 23:55:40 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 13 Jan 2021 23:55:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jan 2021 23:55:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jan 2021 23:55:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jan 2021 23:55:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jan 2021 23:55:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jan 2021 23:55:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jan 2021 23:55:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jan 2021 23:55:46 GMT
EXPOSE 80
# Wed, 13 Jan 2021 23:55:47 GMT
EXPOSE 443
# Wed, 13 Jan 2021 23:55:47 GMT
EXPOSE 2019
# Wed, 13 Jan 2021 23:56:03 GMT
RUN caddy version
# Wed, 13 Jan 2021 23:56:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c124ed0d151a1307812206eec4161e9804c77db85ba840ec7d45bc33bf25acef`  
		Last Modified: Thu, 14 Jan 2021 00:09:34 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d9670a3dfa69d711e77778bae180641069edf70b01eee3587cb3b58c6f9091`  
		Last Modified: Thu, 14 Jan 2021 00:09:52 GMT  
		Size: 16.3 MB (16307704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e85f5144957d7b94c1e0770a5d729479fbbb6abb30c1e8fad73d4b0621a7ac`  
		Last Modified: Thu, 14 Jan 2021 00:09:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3188deca602b712abee415b3c830b4eda39909a2632cd02ca4fd725ba7f5415f`  
		Last Modified: Thu, 14 Jan 2021 00:09:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf888a134df21c7299086dd6e19b9decd248fa28e6858823c9c93b6a38004e00`  
		Last Modified: Thu, 14 Jan 2021 00:09:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee886f5dd5416c025115a9b568f4ccdb55d646baf70af51df77f65185682c260`  
		Last Modified: Thu, 14 Jan 2021 00:09:32 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f5de35d4b9ba97a7823f79b5a1f90a1cc25aafdbb492ffc3202582ea98925b`  
		Last Modified: Thu, 14 Jan 2021 00:09:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f82ceed44af34379ac6644f2575d0f332a13039b60a8fe395195f1422f649f`  
		Last Modified: Thu, 14 Jan 2021 00:09:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1376a8028a57fb7368999c1f91b0a4f41c98923c0ac4222fccdb4e4e68b959c`  
		Last Modified: Thu, 14 Jan 2021 00:09:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832116a3dce559e11031e320446864bfc65aea66f5a5f4a920af087e3db28d2`  
		Last Modified: Thu, 14 Jan 2021 00:09:27 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12220fcac27b241b63d9bbd7b389bf59d8c5b8edc18d325646704fe7c999993e`  
		Last Modified: Thu, 14 Jan 2021 00:09:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644e780eb8777c82e3d0a1baacccfd059c7bf7ff47b3846cb57399733f2da28`  
		Last Modified: Thu, 14 Jan 2021 00:09:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6c8ab724b128c46cc7a60c67b072fead74ea791a0275ae5cdcc5d28f86927e`  
		Last Modified: Thu, 14 Jan 2021 00:09:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48432173e92cc5e546e631a12d3d05b3ae7749b2d1a024d04a57ed89f8a746ec`  
		Last Modified: Thu, 14 Jan 2021 00:09:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e974c8bfaf6d189c7e66cf17b335a348adc8de3811fe703349624507b0c8a`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9998c7eeac899de391fe587610436543215c9b5bb8694885ad678b0072fe81`  
		Last Modified: Thu, 14 Jan 2021 00:09:22 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671afb150632e6b615d24a562f955f57850631d76c03b9f63191f7f0cac20262`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc6746c4e5ba80d375ee895766745cd46896787b48e201104b04ba094dd21c`  
		Last Modified: Thu, 14 Jan 2021 00:09:22 GMT  
		Size: 286.5 KB (286517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583207787ffc504b8838ec2b1a2d994b1bf54b0c8fe26e7cff56e34c438726ee`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:034e3e20762eac42d8248ba526a204bed664f1c1f0ef0426b521ae2e47137416
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826089031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293392087096363f09b0cceb5f945775bd63d56ec9312fe34a63bbb7d54ade8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Jan 2021 23:57:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 13 Jan 2021 23:59:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Jan 2021 23:59:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Jan 2021 23:59:14 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Jan 2021 23:59:15 GMT
VOLUME [c:/config]
# Wed, 13 Jan 2021 23:59:16 GMT
VOLUME [c:/data]
# Wed, 13 Jan 2021 23:59:17 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 13 Jan 2021 23:59:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jan 2021 23:59:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jan 2021 23:59:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jan 2021 23:59:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jan 2021 23:59:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jan 2021 23:59:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jan 2021 23:59:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jan 2021 23:59:23 GMT
EXPOSE 80
# Wed, 13 Jan 2021 23:59:23 GMT
EXPOSE 443
# Wed, 13 Jan 2021 23:59:24 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:00:09 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:00:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28b87abdf6e3be8c33da6b12f1375aea2fa74297da65a841c23f039e5689bbf`  
		Last Modified: Thu, 14 Jan 2021 00:10:12 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ed6dafb20b55ca2dcb4de7a1db1656510aa2648f23f00be3e37375a18a2a6b`  
		Last Modified: Thu, 14 Jan 2021 00:10:18 GMT  
		Size: 21.8 MB (21762420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba37d3037eb80173741da6218a106034d6ba7896dc5f649573d5a1fc087b8102`  
		Last Modified: Thu, 14 Jan 2021 00:10:11 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c5f5ada9e1a6df2043530cb3ab310018509cca67da6c5ba876e31f6dc6c5a`  
		Last Modified: Thu, 14 Jan 2021 00:10:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e66e3e416fcc86941a7c1f47e94b9a42be2b3edd88c65e23d4aa0261f74989`  
		Last Modified: Thu, 14 Jan 2021 00:10:10 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b90913564ebeb758a17403cd0602e5ce3c56155748e513692ae70cce2213`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8578b0a78f1975bc7aeacc49376efb9facdb0d203576ced81e7e3927fb8ed72`  
		Last Modified: Thu, 14 Jan 2021 00:10:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef81ec7cf1113201ee01d28aedbbec62a3101fdb3f8b9de4247ae9a0b58c555`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817ffaa9626f4e46882ac28f2efcd0586061a0baf98688d52402dbb0de03215d`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89364019a3b65364f6b1f0ba723864a6d4cae0bea7656f9ab7d59515d2e34bf`  
		Last Modified: Thu, 14 Jan 2021 00:10:04 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd94f3168a0e1c98cc1440a9f1c12f362c59880b0c60d84b78aea3a0a64087`  
		Last Modified: Thu, 14 Jan 2021 00:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9202b62e65b50cd8eb240a52f5c7d62308134090ca9663989e9721c4f2f7ff1c`  
		Last Modified: Thu, 14 Jan 2021 00:10:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6081d4017544c5d204ffb58282f4441600f01c73bafe75dae71da752d4b90d`  
		Last Modified: Thu, 14 Jan 2021 00:10:06 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe20d79b433436aac1ae29cd8d6ad13fce1527f7a36343d2569008408835c7a`  
		Last Modified: Thu, 14 Jan 2021 00:10:05 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d53536d84b29aa2010d9cd0060330625e0ff43a811f6e6003f904219d3693e`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3eed7ce71e8e377ffe44a8f1c3b07bb5d3977825bd60e34939ab09f56b6b7`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9951f12eddf01971d830855386f82f00dc9ec556897d8c3c1b2f6c9908c5fb`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f0a5b58784c2b79d658ed30acaaa0f78f8d5c7cdbb53935c07bd3dc73f9655`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 250.7 KB (250694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9a287f3f87262639f64d73b8e217de5b0de8440884c0b5a03accbc956ac6de`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1140 bytes)  
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
$ docker pull caddy@sha256:8deffb464f2920d0b3cb805ba3f6a6106bc71a2face4f4056efa08b5caa85302
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.2.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:1aa05c45f9f057ae5d2ad5ef08be5de0904a6b8c209a9a11497d440fa9af912a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f25fca044b231c05994946217aadd9979968d731a4ebd07d530d73b647d55f`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:38 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:40 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c747611b0cf55f036d041767695b58fa1925f9c05be44cfcce2986eb74d359`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 1.3 MB (1308347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c26ac837389243a96fb8980bdd1b20f356358e67edd7601996627c088ef0b35`  
		Last Modified: Wed, 20 Jan 2021 00:59:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a2518408d193daffc6ff6d5697490baaa85641986887231487be9fe68f1762ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636d4ef83bc7844ff0248abe2f8a1785f88758d5895129cf99fa4c6d06d87fd0`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:02 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:54:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:07 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc65b19caa6bb228340e6f077ae9cdfe2043f406acbfa3362822d4ca5d5e187d`  
		Last Modified: Wed, 20 Jan 2021 00:54:55 GMT  
		Size: 1.2 MB (1219246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b09c1cb428400769d6cf1aaf178fd9837e82fb95bf1a83c0165acaae71d654`  
		Last Modified: Wed, 20 Jan 2021 00:54:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d415780a70d42e46c08469cfc989a6aee8db6f17d17fab8d36b81ae2e8bdf3b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfbdbbbbff315a18bd1e5c721616eaf48f1dd19ec7432cc9ab276235d367160`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:57:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:29 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a80fa30f5a386989ee472d7fae71e41674c1ab3de92f99859e9c192b3acc27`  
		Last Modified: Wed, 20 Jan 2021 00:58:11 GMT  
		Size: 1.2 MB (1216917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8436ae47f65ebd6e9a35ff015566f1e7fb5b5cff6e964c57f9186339e09b605`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c36b2da730c995d41ee3fd97784cc726a2e3b781b12ddb81dd1988eb898f4951
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c94d582b3a3aa30831a82a703a1bcebdfdd83feff2f24132e2be536b0a3ae01`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:11 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:55:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:15 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f192934999526403fa968546e18910649e40e31be9f6f0761e3c19b3f9aba782`  
		Last Modified: Wed, 20 Jan 2021 00:55:55 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a6d129b0a1ad6ae430169f27a929e7e46eae7bbd6767ff0b330d815c4642`  
		Last Modified: Wed, 20 Jan 2021 00:55:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:6b15a49d13fc76817bea6d651aa5f3ce02a76b014c9719649737a992817e177b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7571b483316a1b67ecb9c9d8487b09b754ebbff3c9dc64135f33a929ba624f5`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:53 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:53:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:13 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e675b036f1ad255fdd83d544239d423a2fff455e68dfc43027ef68e2b065a4b`  
		Last Modified: Wed, 20 Jan 2021 00:54:32 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7273f42c9a87385fe07231b7a25ec12cb6177067d3be37edfee8b82a0c2ef7e`  
		Last Modified: Wed, 20 Jan 2021 00:54:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:a20e35fd91fc1b962ba0f45f013367528de81855f788e56ff37fa99392be57bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7573bc3d20389c1d2bf6641b598611d2d9ee5b7ab30cd972b033bd122e4877ca`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:19 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:52:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:23 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34eedf22f6a880f728fa376aea356431e62d5680c24644d62518366048e2627c`  
		Last Modified: Wed, 20 Jan 2021 00:53:06 GMT  
		Size: 1.3 MB (1262677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989f3d3ddc7a87144712016ee6dc6988f0e820c38f7486ec780147595c8cc99a`  
		Last Modified: Wed, 20 Jan 2021 00:53:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:4f89d214c6606db62ed6df19ca3a84956261158635c9faeda4be363f0de72a30
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d248c20c5667c462c9cc4c6287cdd800117bd861446923235a833fec2f96ab8c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 02:59:46 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 02:59:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:00:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:00:16 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9d6407cf8a0bdb5da6e67146705c2571b1507f71cf607485323e104218065c`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf6dcfca3d197acb520a9c416b07a067ee01b4205e206d827f1e69010d57714`  
		Last Modified: Wed, 20 Jan 2021 03:05:15 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c80dc50ad2d9bf9c2dab226db26e85525205ba6764b59f697913a5f55d3fea1`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 6.1 MB (6096263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7849a8b41efa28578c568376bd5899a2dd57d816fcb7e9c62890ffd2ed53c167`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:d51ca3c61c65ad51ebf150ff4c6e93eeb2a8cffa3c814ee1963eaa66fbad4a90
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990198063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c2ecedd0c168fc90faddc2e54010cd6f7992215b204e0b4f508b1577e96638`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:00:23 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 03:00:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:01:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:01:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d64f4648cc4581b341636122660b02b3ccd032231cbbadb81f019827ef7bf9b`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a32e9d00d006e76689fc75d434ed7e30fc32b69210943a973b97370d3d49ca`  
		Last Modified: Wed, 20 Jan 2021 03:05:35 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2897d23d0ee16915351cbb6018bc1db87a170739c99027268a21ac4c3bb73cc2`  
		Last Modified: Wed, 20 Jan 2021 03:05:35 GMT  
		Size: 11.5 MB (11505781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b173bcf99b226c215ad649dc07f51d607afab8c99163a5cb62015cc30c9598e`  
		Last Modified: Wed, 20 Jan 2021 03:05:35 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-alpine`

```console
$ docker pull caddy@sha256:70b94b583bec46de25838ea082fb710d051bb5a39011d512d1a5a97886b64c82
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
$ docker pull caddy@sha256:1aa05c45f9f057ae5d2ad5ef08be5de0904a6b8c209a9a11497d440fa9af912a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f25fca044b231c05994946217aadd9979968d731a4ebd07d530d73b647d55f`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:38 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:40 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c747611b0cf55f036d041767695b58fa1925f9c05be44cfcce2986eb74d359`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 1.3 MB (1308347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c26ac837389243a96fb8980bdd1b20f356358e67edd7601996627c088ef0b35`  
		Last Modified: Wed, 20 Jan 2021 00:59:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a2518408d193daffc6ff6d5697490baaa85641986887231487be9fe68f1762ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636d4ef83bc7844ff0248abe2f8a1785f88758d5895129cf99fa4c6d06d87fd0`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:02 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:54:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:07 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc65b19caa6bb228340e6f077ae9cdfe2043f406acbfa3362822d4ca5d5e187d`  
		Last Modified: Wed, 20 Jan 2021 00:54:55 GMT  
		Size: 1.2 MB (1219246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b09c1cb428400769d6cf1aaf178fd9837e82fb95bf1a83c0165acaae71d654`  
		Last Modified: Wed, 20 Jan 2021 00:54:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d415780a70d42e46c08469cfc989a6aee8db6f17d17fab8d36b81ae2e8bdf3b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfbdbbbbff315a18bd1e5c721616eaf48f1dd19ec7432cc9ab276235d367160`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:25 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:57:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:29 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a80fa30f5a386989ee472d7fae71e41674c1ab3de92f99859e9c192b3acc27`  
		Last Modified: Wed, 20 Jan 2021 00:58:11 GMT  
		Size: 1.2 MB (1216917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8436ae47f65ebd6e9a35ff015566f1e7fb5b5cff6e964c57f9186339e09b605`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c36b2da730c995d41ee3fd97784cc726a2e3b781b12ddb81dd1988eb898f4951
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c94d582b3a3aa30831a82a703a1bcebdfdd83feff2f24132e2be536b0a3ae01`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:11 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:55:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:15 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f192934999526403fa968546e18910649e40e31be9f6f0761e3c19b3f9aba782`  
		Last Modified: Wed, 20 Jan 2021 00:55:55 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a6d129b0a1ad6ae430169f27a929e7e46eae7bbd6767ff0b330d815c4642`  
		Last Modified: Wed, 20 Jan 2021 00:55:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:6b15a49d13fc76817bea6d651aa5f3ce02a76b014c9719649737a992817e177b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7571b483316a1b67ecb9c9d8487b09b754ebbff3c9dc64135f33a929ba624f5`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:53 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:53:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:13 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e675b036f1ad255fdd83d544239d423a2fff455e68dfc43027ef68e2b065a4b`  
		Last Modified: Wed, 20 Jan 2021 00:54:32 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7273f42c9a87385fe07231b7a25ec12cb6177067d3be37edfee8b82a0c2ef7e`  
		Last Modified: Wed, 20 Jan 2021 00:54:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:a20e35fd91fc1b962ba0f45f013367528de81855f788e56ff37fa99392be57bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7573bc3d20389c1d2bf6641b598611d2d9ee5b7ab30cd972b033bd122e4877ca`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:19 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 00:52:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:23 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34eedf22f6a880f728fa376aea356431e62d5680c24644d62518366048e2627c`  
		Last Modified: Wed, 20 Jan 2021 00:53:06 GMT  
		Size: 1.3 MB (1262677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989f3d3ddc7a87144712016ee6dc6988f0e820c38f7486ec780147595c8cc99a`  
		Last Modified: Wed, 20 Jan 2021 00:53:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2bd99477d0b874559887b9e655c76545b19f6b41e762ae5af61d0900adf501c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:2.2.1-builder-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:4f89d214c6606db62ed6df19ca3a84956261158635c9faeda4be363f0de72a30
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d248c20c5667c462c9cc4c6287cdd800117bd861446923235a833fec2f96ab8c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 02:59:46 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 02:59:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:00:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:00:16 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9d6407cf8a0bdb5da6e67146705c2571b1507f71cf607485323e104218065c`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf6dcfca3d197acb520a9c416b07a067ee01b4205e206d827f1e69010d57714`  
		Last Modified: Wed, 20 Jan 2021 03:05:15 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c80dc50ad2d9bf9c2dab226db26e85525205ba6764b59f697913a5f55d3fea1`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 6.1 MB (6096263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7849a8b41efa28578c568376bd5899a2dd57d816fcb7e9c62890ffd2ed53c167`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:ac29d767531103a8d1fe3798e0574da8ef5c5d45145a04aad9a2179ff7dfdae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.2.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:d51ca3c61c65ad51ebf150ff4c6e93eeb2a8cffa3c814ee1963eaa66fbad4a90
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990198063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c2ecedd0c168fc90faddc2e54010cd6f7992215b204e0b4f508b1577e96638`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:00:23 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 20 Jan 2021 03:00:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:01:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:01:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d64f4648cc4581b341636122660b02b3ccd032231cbbadb81f019827ef7bf9b`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a32e9d00d006e76689fc75d434ed7e30fc32b69210943a973b97370d3d49ca`  
		Last Modified: Wed, 20 Jan 2021 03:05:35 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2897d23d0ee16915351cbb6018bc1db87a170739c99027268a21ac4c3bb73cc2`  
		Last Modified: Wed, 20 Jan 2021 03:05:35 GMT  
		Size: 11.5 MB (11505781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b173bcf99b226c215ad649dc07f51d607afab8c99163a5cb62015cc30c9598e`  
		Last Modified: Wed, 20 Jan 2021 03:05:35 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore`

```console
$ docker pull caddy@sha256:6e24a2630b9746ff1d6eee2f8f4243de83a2421ae1716789793b9a7f2b02d759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.2.1-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:d609c829f7d4a0747c339fe7dc0f43c53dc981c5c5c974aea1897eed3ac7f971
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461757069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62e3aa62d54d82435bcaf541e63ef826fbb38a40c1a7db894d5fe37948c3d14`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Jan 2021 23:55:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 13 Jan 2021 23:55:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Jan 2021 23:55:37 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Jan 2021 23:55:38 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Jan 2021 23:55:39 GMT
VOLUME [c:/config]
# Wed, 13 Jan 2021 23:55:39 GMT
VOLUME [c:/data]
# Wed, 13 Jan 2021 23:55:40 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 13 Jan 2021 23:55:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jan 2021 23:55:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jan 2021 23:55:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jan 2021 23:55:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jan 2021 23:55:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jan 2021 23:55:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jan 2021 23:55:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jan 2021 23:55:46 GMT
EXPOSE 80
# Wed, 13 Jan 2021 23:55:47 GMT
EXPOSE 443
# Wed, 13 Jan 2021 23:55:47 GMT
EXPOSE 2019
# Wed, 13 Jan 2021 23:56:03 GMT
RUN caddy version
# Wed, 13 Jan 2021 23:56:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c124ed0d151a1307812206eec4161e9804c77db85ba840ec7d45bc33bf25acef`  
		Last Modified: Thu, 14 Jan 2021 00:09:34 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d9670a3dfa69d711e77778bae180641069edf70b01eee3587cb3b58c6f9091`  
		Last Modified: Thu, 14 Jan 2021 00:09:52 GMT  
		Size: 16.3 MB (16307704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e85f5144957d7b94c1e0770a5d729479fbbb6abb30c1e8fad73d4b0621a7ac`  
		Last Modified: Thu, 14 Jan 2021 00:09:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3188deca602b712abee415b3c830b4eda39909a2632cd02ca4fd725ba7f5415f`  
		Last Modified: Thu, 14 Jan 2021 00:09:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf888a134df21c7299086dd6e19b9decd248fa28e6858823c9c93b6a38004e00`  
		Last Modified: Thu, 14 Jan 2021 00:09:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee886f5dd5416c025115a9b568f4ccdb55d646baf70af51df77f65185682c260`  
		Last Modified: Thu, 14 Jan 2021 00:09:32 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f5de35d4b9ba97a7823f79b5a1f90a1cc25aafdbb492ffc3202582ea98925b`  
		Last Modified: Thu, 14 Jan 2021 00:09:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f82ceed44af34379ac6644f2575d0f332a13039b60a8fe395195f1422f649f`  
		Last Modified: Thu, 14 Jan 2021 00:09:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1376a8028a57fb7368999c1f91b0a4f41c98923c0ac4222fccdb4e4e68b959c`  
		Last Modified: Thu, 14 Jan 2021 00:09:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832116a3dce559e11031e320446864bfc65aea66f5a5f4a920af087e3db28d2`  
		Last Modified: Thu, 14 Jan 2021 00:09:27 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12220fcac27b241b63d9bbd7b389bf59d8c5b8edc18d325646704fe7c999993e`  
		Last Modified: Thu, 14 Jan 2021 00:09:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644e780eb8777c82e3d0a1baacccfd059c7bf7ff47b3846cb57399733f2da28`  
		Last Modified: Thu, 14 Jan 2021 00:09:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6c8ab724b128c46cc7a60c67b072fead74ea791a0275ae5cdcc5d28f86927e`  
		Last Modified: Thu, 14 Jan 2021 00:09:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48432173e92cc5e546e631a12d3d05b3ae7749b2d1a024d04a57ed89f8a746ec`  
		Last Modified: Thu, 14 Jan 2021 00:09:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e974c8bfaf6d189c7e66cf17b335a348adc8de3811fe703349624507b0c8a`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9998c7eeac899de391fe587610436543215c9b5bb8694885ad678b0072fe81`  
		Last Modified: Thu, 14 Jan 2021 00:09:22 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671afb150632e6b615d24a562f955f57850631d76c03b9f63191f7f0cac20262`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc6746c4e5ba80d375ee895766745cd46896787b48e201104b04ba094dd21c`  
		Last Modified: Thu, 14 Jan 2021 00:09:22 GMT  
		Size: 286.5 KB (286517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583207787ffc504b8838ec2b1a2d994b1bf54b0c8fe26e7cff56e34c438726ee`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.1-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:034e3e20762eac42d8248ba526a204bed664f1c1f0ef0426b521ae2e47137416
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826089031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293392087096363f09b0cceb5f945775bd63d56ec9312fe34a63bbb7d54ade8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Jan 2021 23:57:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 13 Jan 2021 23:59:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Jan 2021 23:59:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Jan 2021 23:59:14 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Jan 2021 23:59:15 GMT
VOLUME [c:/config]
# Wed, 13 Jan 2021 23:59:16 GMT
VOLUME [c:/data]
# Wed, 13 Jan 2021 23:59:17 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 13 Jan 2021 23:59:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jan 2021 23:59:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jan 2021 23:59:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jan 2021 23:59:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jan 2021 23:59:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jan 2021 23:59:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jan 2021 23:59:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jan 2021 23:59:23 GMT
EXPOSE 80
# Wed, 13 Jan 2021 23:59:23 GMT
EXPOSE 443
# Wed, 13 Jan 2021 23:59:24 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:00:09 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:00:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28b87abdf6e3be8c33da6b12f1375aea2fa74297da65a841c23f039e5689bbf`  
		Last Modified: Thu, 14 Jan 2021 00:10:12 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ed6dafb20b55ca2dcb4de7a1db1656510aa2648f23f00be3e37375a18a2a6b`  
		Last Modified: Thu, 14 Jan 2021 00:10:18 GMT  
		Size: 21.8 MB (21762420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba37d3037eb80173741da6218a106034d6ba7896dc5f649573d5a1fc087b8102`  
		Last Modified: Thu, 14 Jan 2021 00:10:11 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c5f5ada9e1a6df2043530cb3ab310018509cca67da6c5ba876e31f6dc6c5a`  
		Last Modified: Thu, 14 Jan 2021 00:10:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e66e3e416fcc86941a7c1f47e94b9a42be2b3edd88c65e23d4aa0261f74989`  
		Last Modified: Thu, 14 Jan 2021 00:10:10 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b90913564ebeb758a17403cd0602e5ce3c56155748e513692ae70cce2213`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8578b0a78f1975bc7aeacc49376efb9facdb0d203576ced81e7e3927fb8ed72`  
		Last Modified: Thu, 14 Jan 2021 00:10:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef81ec7cf1113201ee01d28aedbbec62a3101fdb3f8b9de4247ae9a0b58c555`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817ffaa9626f4e46882ac28f2efcd0586061a0baf98688d52402dbb0de03215d`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89364019a3b65364f6b1f0ba723864a6d4cae0bea7656f9ab7d59515d2e34bf`  
		Last Modified: Thu, 14 Jan 2021 00:10:04 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd94f3168a0e1c98cc1440a9f1c12f362c59880b0c60d84b78aea3a0a64087`  
		Last Modified: Thu, 14 Jan 2021 00:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9202b62e65b50cd8eb240a52f5c7d62308134090ca9663989e9721c4f2f7ff1c`  
		Last Modified: Thu, 14 Jan 2021 00:10:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6081d4017544c5d204ffb58282f4441600f01c73bafe75dae71da752d4b90d`  
		Last Modified: Thu, 14 Jan 2021 00:10:06 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe20d79b433436aac1ae29cd8d6ad13fce1527f7a36343d2569008408835c7a`  
		Last Modified: Thu, 14 Jan 2021 00:10:05 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d53536d84b29aa2010d9cd0060330625e0ff43a811f6e6003f904219d3693e`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3eed7ce71e8e377ffe44a8f1c3b07bb5d3977825bd60e34939ab09f56b6b7`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9951f12eddf01971d830855386f82f00dc9ec556897d8c3c1b2f6c9908c5fb`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f0a5b58784c2b79d658ed30acaaa0f78f8d5c7cdbb53935c07bd3dc73f9655`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 250.7 KB (250694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9a287f3f87262639f64d73b8e217de5b0de8440884c0b5a03accbc956ac6de`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ed4b7da16eb03d4a307275352d980513a0742a392b59e3f513c7933314a7a1a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:d609c829f7d4a0747c339fe7dc0f43c53dc981c5c5c974aea1897eed3ac7f971
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461757069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62e3aa62d54d82435bcaf541e63ef826fbb38a40c1a7db894d5fe37948c3d14`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Jan 2021 23:55:05 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 13 Jan 2021 23:55:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Jan 2021 23:55:37 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Jan 2021 23:55:38 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Jan 2021 23:55:39 GMT
VOLUME [c:/config]
# Wed, 13 Jan 2021 23:55:39 GMT
VOLUME [c:/data]
# Wed, 13 Jan 2021 23:55:40 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 13 Jan 2021 23:55:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jan 2021 23:55:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jan 2021 23:55:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jan 2021 23:55:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jan 2021 23:55:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jan 2021 23:55:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jan 2021 23:55:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jan 2021 23:55:46 GMT
EXPOSE 80
# Wed, 13 Jan 2021 23:55:47 GMT
EXPOSE 443
# Wed, 13 Jan 2021 23:55:47 GMT
EXPOSE 2019
# Wed, 13 Jan 2021 23:56:03 GMT
RUN caddy version
# Wed, 13 Jan 2021 23:56:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c124ed0d151a1307812206eec4161e9804c77db85ba840ec7d45bc33bf25acef`  
		Last Modified: Thu, 14 Jan 2021 00:09:34 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d9670a3dfa69d711e77778bae180641069edf70b01eee3587cb3b58c6f9091`  
		Last Modified: Thu, 14 Jan 2021 00:09:52 GMT  
		Size: 16.3 MB (16307704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e85f5144957d7b94c1e0770a5d729479fbbb6abb30c1e8fad73d4b0621a7ac`  
		Last Modified: Thu, 14 Jan 2021 00:09:35 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3188deca602b712abee415b3c830b4eda39909a2632cd02ca4fd725ba7f5415f`  
		Last Modified: Thu, 14 Jan 2021 00:09:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf888a134df21c7299086dd6e19b9decd248fa28e6858823c9c93b6a38004e00`  
		Last Modified: Thu, 14 Jan 2021 00:09:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee886f5dd5416c025115a9b568f4ccdb55d646baf70af51df77f65185682c260`  
		Last Modified: Thu, 14 Jan 2021 00:09:32 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f5de35d4b9ba97a7823f79b5a1f90a1cc25aafdbb492ffc3202582ea98925b`  
		Last Modified: Thu, 14 Jan 2021 00:09:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f82ceed44af34379ac6644f2575d0f332a13039b60a8fe395195f1422f649f`  
		Last Modified: Thu, 14 Jan 2021 00:09:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1376a8028a57fb7368999c1f91b0a4f41c98923c0ac4222fccdb4e4e68b959c`  
		Last Modified: Thu, 14 Jan 2021 00:09:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832116a3dce559e11031e320446864bfc65aea66f5a5f4a920af087e3db28d2`  
		Last Modified: Thu, 14 Jan 2021 00:09:27 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12220fcac27b241b63d9bbd7b389bf59d8c5b8edc18d325646704fe7c999993e`  
		Last Modified: Thu, 14 Jan 2021 00:09:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644e780eb8777c82e3d0a1baacccfd059c7bf7ff47b3846cb57399733f2da28`  
		Last Modified: Thu, 14 Jan 2021 00:09:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6c8ab724b128c46cc7a60c67b072fead74ea791a0275ae5cdcc5d28f86927e`  
		Last Modified: Thu, 14 Jan 2021 00:09:27 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48432173e92cc5e546e631a12d3d05b3ae7749b2d1a024d04a57ed89f8a746ec`  
		Last Modified: Thu, 14 Jan 2021 00:09:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e974c8bfaf6d189c7e66cf17b335a348adc8de3811fe703349624507b0c8a`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9998c7eeac899de391fe587610436543215c9b5bb8694885ad678b0072fe81`  
		Last Modified: Thu, 14 Jan 2021 00:09:22 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671afb150632e6b615d24a562f955f57850631d76c03b9f63191f7f0cac20262`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc6746c4e5ba80d375ee895766745cd46896787b48e201104b04ba094dd21c`  
		Last Modified: Thu, 14 Jan 2021 00:09:22 GMT  
		Size: 286.5 KB (286517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583207787ffc504b8838ec2b1a2d994b1bf54b0c8fe26e7cff56e34c438726ee`  
		Last Modified: Thu, 14 Jan 2021 00:09:21 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:2702fbf4d395bce31f1ae835f9714de6f169dd02dae733e7d82cf5a63a331b6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:034e3e20762eac42d8248ba526a204bed664f1c1f0ef0426b521ae2e47137416
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826089031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293392087096363f09b0cceb5f945775bd63d56ec9312fe34a63bbb7d54ade8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Jan 2021 23:57:43 GMT
ENV CADDY_VERSION=v2.2.1
# Wed, 13 Jan 2021 23:59:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.1/caddy_2.2.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e5c5fba6af33a0e1b48cbabc106e907dc7171c2cc337ee5c7cbbad07587dc4970c3f49812b3938dee43209b7fe293c74b36274fd809730ecec0041dd6b1fa93d')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Jan 2021 23:59:13 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Jan 2021 23:59:14 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Jan 2021 23:59:15 GMT
VOLUME [c:/config]
# Wed, 13 Jan 2021 23:59:16 GMT
VOLUME [c:/data]
# Wed, 13 Jan 2021 23:59:17 GMT
LABEL org.opencontainers.image.version=v2.2.1
# Wed, 13 Jan 2021 23:59:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Jan 2021 23:59:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Jan 2021 23:59:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Jan 2021 23:59:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Jan 2021 23:59:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Jan 2021 23:59:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Jan 2021 23:59:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Jan 2021 23:59:23 GMT
EXPOSE 80
# Wed, 13 Jan 2021 23:59:23 GMT
EXPOSE 443
# Wed, 13 Jan 2021 23:59:24 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:00:09 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:00:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28b87abdf6e3be8c33da6b12f1375aea2fa74297da65a841c23f039e5689bbf`  
		Last Modified: Thu, 14 Jan 2021 00:10:12 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ed6dafb20b55ca2dcb4de7a1db1656510aa2648f23f00be3e37375a18a2a6b`  
		Last Modified: Thu, 14 Jan 2021 00:10:18 GMT  
		Size: 21.8 MB (21762420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba37d3037eb80173741da6218a106034d6ba7896dc5f649573d5a1fc087b8102`  
		Last Modified: Thu, 14 Jan 2021 00:10:11 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c5f5ada9e1a6df2043530cb3ab310018509cca67da6c5ba876e31f6dc6c5a`  
		Last Modified: Thu, 14 Jan 2021 00:10:11 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e66e3e416fcc86941a7c1f47e94b9a42be2b3edd88c65e23d4aa0261f74989`  
		Last Modified: Thu, 14 Jan 2021 00:10:10 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f8b90913564ebeb758a17403cd0602e5ce3c56155748e513692ae70cce2213`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8578b0a78f1975bc7aeacc49376efb9facdb0d203576ced81e7e3927fb8ed72`  
		Last Modified: Thu, 14 Jan 2021 00:10:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef81ec7cf1113201ee01d28aedbbec62a3101fdb3f8b9de4247ae9a0b58c555`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817ffaa9626f4e46882ac28f2efcd0586061a0baf98688d52402dbb0de03215d`  
		Last Modified: Thu, 14 Jan 2021 00:10:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89364019a3b65364f6b1f0ba723864a6d4cae0bea7656f9ab7d59515d2e34bf`  
		Last Modified: Thu, 14 Jan 2021 00:10:04 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cd94f3168a0e1c98cc1440a9f1c12f362c59880b0c60d84b78aea3a0a64087`  
		Last Modified: Thu, 14 Jan 2021 00:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9202b62e65b50cd8eb240a52f5c7d62308134090ca9663989e9721c4f2f7ff1c`  
		Last Modified: Thu, 14 Jan 2021 00:10:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6081d4017544c5d204ffb58282f4441600f01c73bafe75dae71da752d4b90d`  
		Last Modified: Thu, 14 Jan 2021 00:10:06 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe20d79b433436aac1ae29cd8d6ad13fce1527f7a36343d2569008408835c7a`  
		Last Modified: Thu, 14 Jan 2021 00:10:05 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d53536d84b29aa2010d9cd0060330625e0ff43a811f6e6003f904219d3693e`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3eed7ce71e8e377ffe44a8f1c3b07bb5d3977825bd60e34939ab09f56b6b7`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9951f12eddf01971d830855386f82f00dc9ec556897d8c3c1b2f6c9908c5fb`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f0a5b58784c2b79d658ed30acaaa0f78f8d5c7cdbb53935c07bd3dc73f9655`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 250.7 KB (250694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9a287f3f87262639f64d73b8e217de5b0de8440884c0b5a03accbc956ac6de`  
		Last Modified: Thu, 14 Jan 2021 00:10:01 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:089eb574cd5464872ede3cd6adb1e12eee92c6f43355794b74438c671ffee975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

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

### `caddy:2.3.0` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
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
$ docker pull caddy@sha256:4f100bdd5a39ead61d937728633a9f24916daecaa04466ea7077cbd6abc5e302
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.3.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a9c9b56a661c9b5342d927f86165d1a9b772d554ca8aebfa83433f8558797cf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d35d90e2260edb2a3ae81be21d5bb810f6e8c3e2f657d379c50109739085d`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:54:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:28 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf586272b896bc536e14f79df0f47ffac7dada3d10bf0d1fbe64b521a66256cb`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 1.2 MB (1219253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882a4ffba9982c6f91bc3c9ebfd5e800ff6d6594501dc5b534ba74b9ea25a44`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:5c42292ac78b4bff9b89f172193d1432ee4d7967dbccfeb21d695511b0443698
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27cc25787f6c9f739fbaff5d1796b878934722eec1e16054b1096d1bc86cb1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:09 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:02:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:02:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48099ada92888d94761c3002930a7638f4d98e6417fb7714cbc302101d5e58a1`  
		Last Modified: Wed, 20 Jan 2021 03:05:54 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70891abc8e284c3890c775002e822a87665807e1a515c900ccfdc3e69be8ca53`  
		Last Modified: Wed, 20 Jan 2021 03:05:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc07c88b14cfe5213c4f2a678d11e9b5a9f7851a0965e2c76197a39f60b6052`  
		Last Modified: Wed, 20 Jan 2021 03:06:07 GMT  
		Size: 6.1 MB (6096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187303bc9eff043ad28ba4c7c5bd6dd3e4c9b277e0671c8786829ce8703e86`  
		Last Modified: Wed, 20 Jan 2021 03:05:55 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:7d61f90c45f2195599804623054c4d8f1a542fbb5a8e9a6a92ffcf71423a9247
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990199069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a61bd522125b0239d3c46f7354d857f7c11b296357e71d219a1de99581cd247`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:45 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:04:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1502aed6d416253ecb5e79d3ce5d893487669f6c970c0425d8d2ecaed8e59fe3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c631491013b9f6de9f8eeec206cfd30fa4cd4e14d9cfa74ebc5789c947dcc914`  
		Last Modified: Wed, 20 Jan 2021 03:06:25 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566636a25817f9babbbd62349ca81edcc01539895974d45365104d5b21aa1d89`  
		Last Modified: Wed, 20 Jan 2021 03:06:38 GMT  
		Size: 11.5 MB (11506780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6a3485f832199dea4cf806e302207c6f6a68b1a96a41cf26dd0ba7fc498d3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:dbc256b175ab3876444324a0ef84a770df364a326abe2df2896802097fa1b131
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
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a9c9b56a661c9b5342d927f86165d1a9b772d554ca8aebfa83433f8558797cf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d35d90e2260edb2a3ae81be21d5bb810f6e8c3e2f657d379c50109739085d`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:54:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:28 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf586272b896bc536e14f79df0f47ffac7dada3d10bf0d1fbe64b521a66256cb`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 1.2 MB (1219253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882a4ffba9982c6f91bc3c9ebfd5e800ff6d6594501dc5b534ba74b9ea25a44`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2ce56ddd0620461295b259fb7aeeb7ac68be5492cb47442bead1552fd9084e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:5c42292ac78b4bff9b89f172193d1432ee4d7967dbccfeb21d695511b0443698
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27cc25787f6c9f739fbaff5d1796b878934722eec1e16054b1096d1bc86cb1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:09 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:02:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:02:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48099ada92888d94761c3002930a7638f4d98e6417fb7714cbc302101d5e58a1`  
		Last Modified: Wed, 20 Jan 2021 03:05:54 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70891abc8e284c3890c775002e822a87665807e1a515c900ccfdc3e69be8ca53`  
		Last Modified: Wed, 20 Jan 2021 03:05:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc07c88b14cfe5213c4f2a678d11e9b5a9f7851a0965e2c76197a39f60b6052`  
		Last Modified: Wed, 20 Jan 2021 03:06:07 GMT  
		Size: 6.1 MB (6096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187303bc9eff043ad28ba4c7c5bd6dd3e4c9b277e0671c8786829ce8703e86`  
		Last Modified: Wed, 20 Jan 2021 03:05:55 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9a6b63e9787e6bac54fc8c544f9559cd0be8c251eaeb63ee1ea475d9f23e4d8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:7d61f90c45f2195599804623054c4d8f1a542fbb5a8e9a6a92ffcf71423a9247
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990199069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a61bd522125b0239d3c46f7354d857f7c11b296357e71d219a1de99581cd247`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:45 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:04:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1502aed6d416253ecb5e79d3ce5d893487669f6c970c0425d8d2ecaed8e59fe3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c631491013b9f6de9f8eeec206cfd30fa4cd4e14d9cfa74ebc5789c947dcc914`  
		Last Modified: Wed, 20 Jan 2021 03:06:25 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566636a25817f9babbbd62349ca81edcc01539895974d45365104d5b21aa1d89`  
		Last Modified: Wed, 20 Jan 2021 03:06:38 GMT  
		Size: 11.5 MB (11506780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6a3485f832199dea4cf806e302207c6f6a68b1a96a41cf26dd0ba7fc498d3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore`

```console
$ docker pull caddy@sha256:5bbc9b2c2450a7471b4997ba53f82c8283a79137dc88f1813a492b054d076b9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.3.0-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:abecf61dde479eb83f03aadca4ce1c7c981ba8ab6a290667fd76a7dbf1105bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:2.3.0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:08473cebef31a1a368655af46bdef8b775914f10527be9200df9d398451df182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:2.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
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
$ docker pull caddy@sha256:4f100bdd5a39ead61d937728633a9f24916daecaa04466ea7077cbd6abc5e302
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a9c9b56a661c9b5342d927f86165d1a9b772d554ca8aebfa83433f8558797cf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d35d90e2260edb2a3ae81be21d5bb810f6e8c3e2f657d379c50109739085d`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:54:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:28 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf586272b896bc536e14f79df0f47ffac7dada3d10bf0d1fbe64b521a66256cb`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 1.2 MB (1219253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882a4ffba9982c6f91bc3c9ebfd5e800ff6d6594501dc5b534ba74b9ea25a44`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:5c42292ac78b4bff9b89f172193d1432ee4d7967dbccfeb21d695511b0443698
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27cc25787f6c9f739fbaff5d1796b878934722eec1e16054b1096d1bc86cb1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:09 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:02:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:02:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48099ada92888d94761c3002930a7638f4d98e6417fb7714cbc302101d5e58a1`  
		Last Modified: Wed, 20 Jan 2021 03:05:54 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70891abc8e284c3890c775002e822a87665807e1a515c900ccfdc3e69be8ca53`  
		Last Modified: Wed, 20 Jan 2021 03:05:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc07c88b14cfe5213c4f2a678d11e9b5a9f7851a0965e2c76197a39f60b6052`  
		Last Modified: Wed, 20 Jan 2021 03:06:07 GMT  
		Size: 6.1 MB (6096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187303bc9eff043ad28ba4c7c5bd6dd3e4c9b277e0671c8786829ce8703e86`  
		Last Modified: Wed, 20 Jan 2021 03:05:55 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:7d61f90c45f2195599804623054c4d8f1a542fbb5a8e9a6a92ffcf71423a9247
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990199069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a61bd522125b0239d3c46f7354d857f7c11b296357e71d219a1de99581cd247`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:45 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:04:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1502aed6d416253ecb5e79d3ce5d893487669f6c970c0425d8d2ecaed8e59fe3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c631491013b9f6de9f8eeec206cfd30fa4cd4e14d9cfa74ebc5789c947dcc914`  
		Last Modified: Wed, 20 Jan 2021 03:06:25 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566636a25817f9babbbd62349ca81edcc01539895974d45365104d5b21aa1d89`  
		Last Modified: Wed, 20 Jan 2021 03:06:38 GMT  
		Size: 11.5 MB (11506780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6a3485f832199dea4cf806e302207c6f6a68b1a96a41cf26dd0ba7fc498d3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:dbc256b175ab3876444324a0ef84a770df364a326abe2df2896802097fa1b131
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
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a9c9b56a661c9b5342d927f86165d1a9b772d554ca8aebfa83433f8558797cf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d35d90e2260edb2a3ae81be21d5bb810f6e8c3e2f657d379c50109739085d`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:54:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:28 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf586272b896bc536e14f79df0f47ffac7dada3d10bf0d1fbe64b521a66256cb`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 1.2 MB (1219253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882a4ffba9982c6f91bc3c9ebfd5e800ff6d6594501dc5b534ba74b9ea25a44`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2ce56ddd0620461295b259fb7aeeb7ac68be5492cb47442bead1552fd9084e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:5c42292ac78b4bff9b89f172193d1432ee4d7967dbccfeb21d695511b0443698
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27cc25787f6c9f739fbaff5d1796b878934722eec1e16054b1096d1bc86cb1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:09 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:02:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:02:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48099ada92888d94761c3002930a7638f4d98e6417fb7714cbc302101d5e58a1`  
		Last Modified: Wed, 20 Jan 2021 03:05:54 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70891abc8e284c3890c775002e822a87665807e1a515c900ccfdc3e69be8ca53`  
		Last Modified: Wed, 20 Jan 2021 03:05:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc07c88b14cfe5213c4f2a678d11e9b5a9f7851a0965e2c76197a39f60b6052`  
		Last Modified: Wed, 20 Jan 2021 03:06:07 GMT  
		Size: 6.1 MB (6096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187303bc9eff043ad28ba4c7c5bd6dd3e4c9b277e0671c8786829ce8703e86`  
		Last Modified: Wed, 20 Jan 2021 03:05:55 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9a6b63e9787e6bac54fc8c544f9559cd0be8c251eaeb63ee1ea475d9f23e4d8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:7d61f90c45f2195599804623054c4d8f1a542fbb5a8e9a6a92ffcf71423a9247
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990199069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a61bd522125b0239d3c46f7354d857f7c11b296357e71d219a1de99581cd247`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:45 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:04:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1502aed6d416253ecb5e79d3ce5d893487669f6c970c0425d8d2ecaed8e59fe3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c631491013b9f6de9f8eeec206cfd30fa4cd4e14d9cfa74ebc5789c947dcc914`  
		Last Modified: Wed, 20 Jan 2021 03:06:25 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566636a25817f9babbbd62349ca81edcc01539895974d45365104d5b21aa1d89`  
		Last Modified: Wed, 20 Jan 2021 03:06:38 GMT  
		Size: 11.5 MB (11506780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6a3485f832199dea4cf806e302207c6f6a68b1a96a41cf26dd0ba7fc498d3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:5bbc9b2c2450a7471b4997ba53f82c8283a79137dc88f1813a492b054d076b9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:abecf61dde479eb83f03aadca4ce1c7c981ba8ab6a290667fd76a7dbf1105bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:08473cebef31a1a368655af46bdef8b775914f10527be9200df9d398451df182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
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
$ docker pull caddy@sha256:4f100bdd5a39ead61d937728633a9f24916daecaa04466ea7077cbd6abc5e302
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a9c9b56a661c9b5342d927f86165d1a9b772d554ca8aebfa83433f8558797cf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d35d90e2260edb2a3ae81be21d5bb810f6e8c3e2f657d379c50109739085d`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:54:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:28 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf586272b896bc536e14f79df0f47ffac7dada3d10bf0d1fbe64b521a66256cb`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 1.2 MB (1219253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882a4ffba9982c6f91bc3c9ebfd5e800ff6d6594501dc5b534ba74b9ea25a44`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:5c42292ac78b4bff9b89f172193d1432ee4d7967dbccfeb21d695511b0443698
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27cc25787f6c9f739fbaff5d1796b878934722eec1e16054b1096d1bc86cb1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:09 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:02:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:02:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48099ada92888d94761c3002930a7638f4d98e6417fb7714cbc302101d5e58a1`  
		Last Modified: Wed, 20 Jan 2021 03:05:54 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70891abc8e284c3890c775002e822a87665807e1a515c900ccfdc3e69be8ca53`  
		Last Modified: Wed, 20 Jan 2021 03:05:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc07c88b14cfe5213c4f2a678d11e9b5a9f7851a0965e2c76197a39f60b6052`  
		Last Modified: Wed, 20 Jan 2021 03:06:07 GMT  
		Size: 6.1 MB (6096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187303bc9eff043ad28ba4c7c5bd6dd3e4c9b277e0671c8786829ce8703e86`  
		Last Modified: Wed, 20 Jan 2021 03:05:55 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:7d61f90c45f2195599804623054c4d8f1a542fbb5a8e9a6a92ffcf71423a9247
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990199069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a61bd522125b0239d3c46f7354d857f7c11b296357e71d219a1de99581cd247`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:45 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:04:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1502aed6d416253ecb5e79d3ce5d893487669f6c970c0425d8d2ecaed8e59fe3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c631491013b9f6de9f8eeec206cfd30fa4cd4e14d9cfa74ebc5789c947dcc914`  
		Last Modified: Wed, 20 Jan 2021 03:06:25 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566636a25817f9babbbd62349ca81edcc01539895974d45365104d5b21aa1d89`  
		Last Modified: Wed, 20 Jan 2021 03:06:38 GMT  
		Size: 11.5 MB (11506780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6a3485f832199dea4cf806e302207c6f6a68b1a96a41cf26dd0ba7fc498d3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:dbc256b175ab3876444324a0ef84a770df364a326abe2df2896802097fa1b131
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
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
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
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
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
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a9c9b56a661c9b5342d927f86165d1a9b772d554ca8aebfa83433f8558797cf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114673366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d35d90e2260edb2a3ae81be21d5bb810f6e8c3e2f657d379c50109739085d`
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
# Wed, 20 Jan 2021 00:19:22 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:46 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:53 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:53:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:54:00 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:54:21 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:54:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:54:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:54:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:54:28 GMT
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
	-	`sha256:9f2aa5ec6d8954c0f817209f1dbbf5b46ac3bd5d2c6085deecba965a709a5fec`  
		Last Modified: Wed, 20 Jan 2021 00:36:00 GMT  
		Size: 102.6 MB (102639302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c85d33cb873133645de906a79c58642723962c47c4e2adebfedf40f07d5d37`  
		Last Modified: Wed, 20 Jan 2021 00:35:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4b1168c364706311edf5b8afd73cb84153b57d2a3ec2db6064089eba8c67d`  
		Last Modified: Wed, 20 Jan 2021 00:54:57 GMT  
		Size: 7.9 MB (7928960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf586272b896bc536e14f79df0f47ffac7dada3d10bf0d1fbe64b521a66256cb`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 1.2 MB (1219253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882a4ffba9982c6f91bc3c9ebfd5e800ff6d6594501dc5b534ba74b9ea25a44`  
		Last Modified: Wed, 20 Jan 2021 00:55:06 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
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
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
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
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
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
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
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
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
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
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
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
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
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
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
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
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2ce56ddd0620461295b259fb7aeeb7ac68be5492cb47442bead1552fd9084e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:5c42292ac78b4bff9b89f172193d1432ee4d7967dbccfeb21d695511b0443698
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2615139382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27cc25787f6c9f739fbaff5d1796b878934722eec1e16054b1096d1bc86cb1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:22:28 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:27:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 00:27:55 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 02:59:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 02:59:45 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:09 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:02:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:02:38 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c609367cccd17e780fe681d808c4e97dd7f6d3090a7bdc688bb29892988d05`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b7f8de1342403844852476ff328591cdc5f37ccabf5d3367cb10ba73eb250`  
		Last Modified: Wed, 20 Jan 2021 02:27:44 GMT  
		Size: 138.5 MB (138501105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a0672040817e88085db591aa81b3cdf693aea735f6bb878c0c23e828c81715`  
		Last Modified: Wed, 20 Jan 2021 02:27:13 GMT  
		Size: 1.5 KB (1458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316414a79e2eec6998f7088bf92b20c74d1747fe0a6fa69375bad0e1bdcfb424`  
		Last Modified: Wed, 20 Jan 2021 03:05:17 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7820ee28454240a57c1b593d74d17f761d8cd06ac6a2bb4a68ad856b1ea96c0`  
		Last Modified: Wed, 20 Jan 2021 03:05:16 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48099ada92888d94761c3002930a7638f4d98e6417fb7714cbc302101d5e58a1`  
		Last Modified: Wed, 20 Jan 2021 03:05:54 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70891abc8e284c3890c775002e822a87665807e1a515c900ccfdc3e69be8ca53`  
		Last Modified: Wed, 20 Jan 2021 03:05:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc07c88b14cfe5213c4f2a678d11e9b5a9f7851a0965e2c76197a39f60b6052`  
		Last Modified: Wed, 20 Jan 2021 03:06:07 GMT  
		Size: 6.1 MB (6096329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78187303bc9eff043ad28ba4c7c5bd6dd3e4c9b277e0671c8786829ce8703e86`  
		Last Modified: Wed, 20 Jan 2021 03:05:55 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9a6b63e9787e6bac54fc8c544f9559cd0be8c251eaeb63ee1ea475d9f23e4d8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:7d61f90c45f2195599804623054c4d8f1a542fbb5a8e9a6a92ffcf71423a9247
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990199069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a61bd522125b0239d3c46f7354d857f7c11b296357e71d219a1de99581cd247`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 20 Jan 2021 00:57:40 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 01:25:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6e8f680118d9dfbd7ee61ed2b3d319f278d41de5757b6e30ed190fa9c3ee5767'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 20 Jan 2021 01:25:50 GMT
WORKDIR C:\gopath
# Wed, 20 Jan 2021 03:00:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 20 Jan 2021 03:00:22 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 03:02:45 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 03:02:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 03:04:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 20 Jan 2021 03:04:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210cf15f1b3a468cc8e664d666c5d14d3f1d1448ec127981429442f1b2d866d`  
		Last Modified: Wed, 20 Jan 2021 02:28:07 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b1b32708c8bf626394cf363c4ac37333d8f80334c44ada24e4a068bab0264`  
		Last Modified: Wed, 20 Jan 2021 02:28:38 GMT  
		Size: 143.9 MB (143939803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e728c038832624a843740f0c65492adb7cb0fec29831bf69734f25758aef5`  
		Last Modified: Wed, 20 Jan 2021 02:28:05 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bc1adf6c08c0917b21ef949933f755b3d840cb103802a168122da9874b4202`  
		Last Modified: Wed, 20 Jan 2021 03:05:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136abac90c1d5ad813db0a0426e4784eabc6b65b44101dccf24314ed1c14bda8`  
		Last Modified: Wed, 20 Jan 2021 03:05:34 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1502aed6d416253ecb5e79d3ce5d893487669f6c970c0425d8d2ecaed8e59fe3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c631491013b9f6de9f8eeec206cfd30fa4cd4e14d9cfa74ebc5789c947dcc914`  
		Last Modified: Wed, 20 Jan 2021 03:06:25 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566636a25817f9babbbd62349ca81edcc01539895974d45365104d5b21aa1d89`  
		Last Modified: Wed, 20 Jan 2021 03:06:38 GMT  
		Size: 11.5 MB (11506780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6a3485f832199dea4cf806e302207c6f6a68b1a96a41cf26dd0ba7fc498d3`  
		Last Modified: Wed, 20 Jan 2021 03:06:24 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:089eb574cd5464872ede3cd6adb1e12eee92c6f43355794b74438c671ffee975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

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

### `caddy:latest` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:5bbc9b2c2450a7471b4997ba53f82c8283a79137dc88f1813a492b054d076b9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:abecf61dde479eb83f03aadca4ce1c7c981ba8ab6a290667fd76a7dbf1105bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:de839e0815b0a64817e61c71de6127bfc07914bb69f87e8408e643af10877328
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2461830878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40640a52040a4245cca4882fc1e070c53ded8b097c9200d6817927ba384d4407`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:55:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:02:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:02:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:03:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:03:01 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:03:02 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:03:03 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:03:03 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:03:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:03:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:03:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:03:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:03:09 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:03:10 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:03:26 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:03:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e6ce3956b2be5c16af8c4b12fb9eee40a47169a238e2ef8cb910eea6f6a86e`  
		Last Modified: Thu, 14 Jan 2021 00:09:40 GMT  
		Size: 9.4 MB (9370292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ace9d6991a65c9a920c33512761b565801eb9b5db738b41e18b582195bc0437`  
		Last Modified: Thu, 14 Jan 2021 00:11:32 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac05c73067e06026b63884d2b0ceecc7bfacb99a453af02c6a0868528ac912`  
		Last Modified: Thu, 14 Jan 2021 00:11:35 GMT  
		Size: 16.4 MB (16392257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b6c4adde3cc3d3e32fe5549d3dea1a2216348b2d97fae69675b6eb7b3f309`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e765211ebb418fe8b27582dbaabf0486499eb2ccd591809893c71655a671bfe`  
		Last Modified: Thu, 14 Jan 2021 00:11:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731a2a977bca2f5da7bc83330664f2e41bf76620a188990374b8c3506f6a7779`  
		Last Modified: Thu, 14 Jan 2021 00:11:28 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fac4d340ec37627761b8ae0a5418ae1fbc95f883bf3d2ab94212f6be113ecde`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d9917863b6ffa78ad654c2658efaef97774e1d238b208b45b430a4327234`  
		Last Modified: Thu, 14 Jan 2021 00:11:27 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7157e44941a360dfe52e95269c91abc19d34c68d59525cfbe38abd16a62a7b38`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f687a5918c96313c6f725550d164c3b5c5727c8dab0fb262d32061cbc3531c3`  
		Last Modified: Thu, 14 Jan 2021 00:11:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8eb7df7525322bb70878976063664f7b4cca0d57cf6ad2dd2314e4ec86035a`  
		Last Modified: Thu, 14 Jan 2021 00:11:25 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2412a0df7d8e2af00ae106f91f34fdbe43ff37fbce05f7aad93337f5e43d62`  
		Last Modified: Thu, 14 Jan 2021 00:11:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fda527bf8c7062b86fc263da411b54c3bbf3514327f842c99c344970197998`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e813b50511cd7ce703252be8d3acd03a640ccc6d5f77fca0de4817699d9a8f0`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97840cd7ebfa98613147c2a4c98663d64ebe1616cc1e746c59403444f443c63b`  
		Last Modified: Thu, 14 Jan 2021 00:11:23 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36419b63a395c8d53fbc2751314f3ae78746df2163d2795cc6601c0e8286e6de`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e0d2113b0eaf06dbcb1d47f151b1634149a5279c4e1826257a0440e388c379`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e44705418f08c2ea5b58e8958be7b17e1056fdd1cb3e0ac76d169577f83dfd`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613471c47f93daf8cf5c203eba41926449d587028540640a60864d2b8070444a`  
		Last Modified: Thu, 14 Jan 2021 00:11:20 GMT  
		Size: 275.7 KB (275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85d427824d62b9858e31e20e9eece84c0544d2baafa60c9af3373c5358d6db`  
		Last Modified: Thu, 14 Jan 2021 00:11:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:08473cebef31a1a368655af46bdef8b775914f10527be9200df9d398451df182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:a95daaf163b6206c31bd5a9fefe535e199796f81dcd7eab682df687a2016f3ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5826167615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb6fe190c1d40eeebb3d48201b9d03df7a5f0c87d3ba6226b1004504e9e287`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 23:57:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Jan 2021 00:03:41 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 14 Jan 2021 00:05:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Jan 2021 00:05:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Jan 2021 00:05:12 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Jan 2021 00:05:13 GMT
VOLUME [c:/config]
# Thu, 14 Jan 2021 00:05:14 GMT
VOLUME [c:/data]
# Thu, 14 Jan 2021 00:05:15 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 14 Jan 2021 00:05:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Jan 2021 00:05:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Jan 2021 00:05:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Jan 2021 00:05:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Jan 2021 00:05:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Jan 2021 00:05:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Jan 2021 00:05:21 GMT
EXPOSE 80
# Thu, 14 Jan 2021 00:05:22 GMT
EXPOSE 443
# Thu, 14 Jan 2021 00:05:23 GMT
EXPOSE 2019
# Thu, 14 Jan 2021 00:06:10 GMT
RUN caddy version
# Thu, 14 Jan 2021 00:06:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ab8111d5c5970d277cc720aa8b29d9a8929b6c0ed278f6d3baf0abf3a5c283`  
		Last Modified: Thu, 14 Jan 2021 00:10:25 GMT  
		Size: 10.2 MB (10161407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbbd4a3517a3e193644d8a9898ba2f50513b1beaf3f5e9689251145863a7223`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4126f87d2fce56ced828634969035d1897145822d09845feac67f7875601d6`  
		Last Modified: Thu, 14 Jan 2021 00:12:34 GMT  
		Size: 21.8 MB (21838247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef97a5d3119fca76ed34dac487bec7550646029f68f221d679350fcbba50bae`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d4c368c88dc8321865eca56ac8d45771c31e8adc870f4be14376ba4485807`  
		Last Modified: Thu, 14 Jan 2021 00:12:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c28a06a7d063d3d3cb6439a248c19aa743448cd057b6e1955a673f8130e1ee`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0054b245b8193dbbd656c99ccdb315c0f9b685eff6edbb6ed07eb90aa6b113a3`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0ed80aa1b02523018d619bf17139788621800c16d15ac388bb65b7660d368`  
		Last Modified: Thu, 14 Jan 2021 00:12:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52af04661019721e096d89b055d565982b8f0b342c4b1b4a847529f20b209546`  
		Last Modified: Thu, 14 Jan 2021 00:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b6e926bea3b9f9a8853e4be32181b75be97d5e430e45337fd063f0aee784bf`  
		Last Modified: Thu, 14 Jan 2021 00:12:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc5dd85c535f4866f5a00f179dffc5473da3c500ab31326bfd71c2ff1a48c59`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5048f14b9e8f2e82ae7a81ef1b42359b98dbf3ed743cb3a5da805393df979cf`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334073bfe9b6f1f64b1405c7da17e07bc8d32a586d2a0352f72def2e10a196af`  
		Last Modified: Thu, 14 Jan 2021 00:12:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6149e51c45c48dc3d10d8017bb209b066f3567342568725e8816e9cab588b9`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fb1a090761c6a1c8cd2b5846400a8ff0879c50e6df8e6ffcb2647b312fa1a`  
		Last Modified: Thu, 14 Jan 2021 00:11:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f8e5f898b74d4c8116bc0ef43023da55b8e9d6ea558c259ac507ab98512e22`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3a01455bd5bb8fe621f0458e773a9d589b1ec97c7531cbe0ba06c459aad58`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10548a36a748b3d59e79857d64fa321af0a803d8d98c1ca668ef19cca9df3022`  
		Last Modified: Thu, 14 Jan 2021 00:11:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eaa62b592ca108e8599ec9769a20acb86a8532f82bb8504fb4c311b53968d1`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 253.5 KB (253489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542abf7478499e56d7b85ec8d24eadb385d11de89ef946d5c0e9d89060c70262`  
		Last Modified: Thu, 14 Jan 2021 00:11:56 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
