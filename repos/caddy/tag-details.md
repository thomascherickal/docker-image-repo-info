<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2016`](#caddy2-builder-windowsservercore-ltsc2016)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:2.3.0`](#caddy230)
-	[`caddy:2.3.0-alpine`](#caddy230-alpine)
-	[`caddy:2.3.0-builder`](#caddy230-builder)
-	[`caddy:2.3.0-builder-alpine`](#caddy230-builder-alpine)
-	[`caddy:2.3.0-builder-windowsservercore-1809`](#caddy230-builder-windowsservercore-1809)
-	[`caddy:2.3.0-builder-windowsservercore-ltsc2016`](#caddy230-builder-windowsservercore-ltsc2016)
-	[`caddy:2.3.0-windowsservercore`](#caddy230-windowsservercore)
-	[`caddy:2.3.0-windowsservercore-1809`](#caddy230-windowsservercore-1809)
-	[`caddy:2.3.0-windowsservercore-ltsc2016`](#caddy230-windowsservercore-ltsc2016)
-	[`caddy:2.4.0-beta.1`](#caddy240-beta1)
-	[`caddy:2.4.0-beta.1-alpine`](#caddy240-beta1-alpine)
-	[`caddy:2.4.0-beta.1-builder`](#caddy240-beta1-builder)
-	[`caddy:2.4.0-beta.1-builder-alpine`](#caddy240-beta1-builder-alpine)
-	[`caddy:2.4.0-beta.1-builder-windowsservercore-1809`](#caddy240-beta1-builder-windowsservercore-1809)
-	[`caddy:2.4.0-beta.1-builder-windowsservercore-ltsc2016`](#caddy240-beta1-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.0-beta.1-windowsservercore`](#caddy240-beta1-windowsservercore)
-	[`caddy:2.4.0-beta.1-windowsservercore-1809`](#caddy240-beta1-windowsservercore-1809)
-	[`caddy:2.4.0-beta.1-windowsservercore-ltsc2016`](#caddy240-beta1-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:9485932040de498b47cf0b6cc5d23cbbfd6282e5ff4884b04413cfda0e642661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:d0b43ebda8fd47409cec98d5f3c3b4c60bfc6bca35338313c002dc64c2283055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88588539bb905b66ad7f78f35b915f2daf56ec49fd5f20019793e9dbd9747497`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:10:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:10:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:10:52 GMT
ENV CADDY_VERSION=v2.3.0
# Sat, 06 Mar 2021 08:10:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:10:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:10:59 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:10:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296b24b4efd312d2a5e0a24a29635cf8aa098c9c3e50ca6566741a54b2794b`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 300.0 KB (300027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0836949366398b595edf3fde04aff8f2a0c0f4c1ea35372e070f4bf27ce59`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7383a05b49b6f752da622ff9a170dccd483a982060cc06a6be10d6312d32a0`  
		Last Modified: Sat, 06 Mar 2021 08:11:52 GMT  
		Size: 11.6 MB (11622385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701a0726354caf82c1c4be1f558173acf8b6604f7b4118a1097b98424256bd`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c03423186b55d3813eb09d04dc53106635be68cfb5969c12109e08cff9aa2cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569b44d4318ddaf5248442e91df11b525d9ccaf230b7efd78c6ce6ef08281ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:07:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:07:11 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:07:11 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:07:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:07:18 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:07:19 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:07:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:07:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:07:26 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:07:27 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:07:28 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:07:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:07:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9d7c4e3e67f9f36b119476dce4a4951c76aca8f9848b7cc600797ce9a5dbb5`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0438df6797a38cba7f30dd40d58d68e90cf6f6a4ece0a3352142ef610796d1`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1886901d622dcb0b11ff563e6eca542fec29b60ae60c1bf82c8d7271fbcb8`  
		Last Modified: Wed, 24 Feb 2021 21:08:13 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f6d93c8b87b0adc5fdfbfb465ceb4e8c5ccbfe7e75288a0b6247b287bd1d19`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35efa62036c16d5ac4716ce79b11c0505538236542b982ce31e580044712c961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e584e1be15b38bc7eddfd01bedf8038c9b6eb1d20a21df121376bc0878fa2b5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:20:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:20:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:20:25 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:20:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:20:32 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:20:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:20:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:20:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:20:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:20:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:20:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:20:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:20:41 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:20:41 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:20:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38341eca332cf74b9be3ce81ca1d45dfb58d85d6d26b7e95c316e6c9bb29ee72`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 299.2 KB (299205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc65ce8d47b334515d1e1114419a952c7a20fde643e2cb7d7fba90886eb905`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dac8b9094b9d9fb88438fba0a9603978bb1779e919ca8adf8673ef932f74e5`  
		Last Modified: Wed, 24 Feb 2021 21:21:23 GMT  
		Size: 10.9 MB (10925347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114ebf580e52effa6a3b734370fc33000e5a7439f0b0b2b275ffaca7483dd32`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9629cb7ae3d67bb1da05e2a4fa565c7549f1d0df99f27e50987ad0414fa275a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0888c16cdeddffbcaf6f274289f92000cb7e408a60c2788e1cecce57fb4f54d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:33:39 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:33:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:33:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:33:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:33:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:33:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:33:49 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:33:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:33:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:33:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:33:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:33:58 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:33:59 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c560f04d39148af03b91ee7707d8a25136794128fdc0eb1a28ee5a9c7ec5`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 300.4 KB (300351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bb894d60771907a615f58e2c0b5873da52637bf52500990e34621581a232d7`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c61561fb1545eb44bb540b09bf7ce497aa3618f51b8dd8013e161cbe6b595d`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d97783fa5ecc238f39ccba3a47e00bbef6ee3ac8db0ad07989b7f65fac81`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:247ebfeff707410bb47d0a0501aee685d43129a4fab344f361ca1430c28a4058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9eef5ad7357ccba137393d95be15feb69c0fb5bf08d5a63bdd1d15f0a957a92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:19:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:19:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:19:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:19:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:19:32 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:19:37 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:19:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:19:40 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866813d62eb8e73b5cfc9e73e48928d678fcad6123ca0697fdc6ff6faf0c91e`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 300.5 KB (300478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8052626100230d16d27888d060e65aaf770add1ae10f69a8f03a903d274ec2`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6a465134a658869ad61a0ea92cf2775ffd82e4cd1d0e2246f24abd0ac95613`  
		Last Modified: Wed, 24 Feb 2021 21:20:17 GMT  
		Size: 11.3 MB (11272060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fffed8a5a7c6c9efd387b3b851eb42ba3b176b5614156a8f2b5ca6dbfe56e7`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:30cf6a3da8365c2d9344adfc42b33a5b6e01dc4943c75b0132d556d12bd5f995
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
$ docker pull caddy@sha256:d0b43ebda8fd47409cec98d5f3c3b4c60bfc6bca35338313c002dc64c2283055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88588539bb905b66ad7f78f35b915f2daf56ec49fd5f20019793e9dbd9747497`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:10:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:10:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:10:52 GMT
ENV CADDY_VERSION=v2.3.0
# Sat, 06 Mar 2021 08:10:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:10:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:10:59 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:10:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296b24b4efd312d2a5e0a24a29635cf8aa098c9c3e50ca6566741a54b2794b`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 300.0 KB (300027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0836949366398b595edf3fde04aff8f2a0c0f4c1ea35372e070f4bf27ce59`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7383a05b49b6f752da622ff9a170dccd483a982060cc06a6be10d6312d32a0`  
		Last Modified: Sat, 06 Mar 2021 08:11:52 GMT  
		Size: 11.6 MB (11622385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701a0726354caf82c1c4be1f558173acf8b6604f7b4118a1097b98424256bd`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c03423186b55d3813eb09d04dc53106635be68cfb5969c12109e08cff9aa2cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569b44d4318ddaf5248442e91df11b525d9ccaf230b7efd78c6ce6ef08281ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:07:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:07:11 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:07:11 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:07:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:07:18 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:07:19 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:07:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:07:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:07:26 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:07:27 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:07:28 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:07:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:07:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9d7c4e3e67f9f36b119476dce4a4951c76aca8f9848b7cc600797ce9a5dbb5`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0438df6797a38cba7f30dd40d58d68e90cf6f6a4ece0a3352142ef610796d1`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1886901d622dcb0b11ff563e6eca542fec29b60ae60c1bf82c8d7271fbcb8`  
		Last Modified: Wed, 24 Feb 2021 21:08:13 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f6d93c8b87b0adc5fdfbfb465ceb4e8c5ccbfe7e75288a0b6247b287bd1d19`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35efa62036c16d5ac4716ce79b11c0505538236542b982ce31e580044712c961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e584e1be15b38bc7eddfd01bedf8038c9b6eb1d20a21df121376bc0878fa2b5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:20:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:20:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:20:25 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:20:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:20:32 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:20:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:20:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:20:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:20:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:20:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:20:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:20:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:20:41 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:20:41 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:20:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38341eca332cf74b9be3ce81ca1d45dfb58d85d6d26b7e95c316e6c9bb29ee72`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 299.2 KB (299205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc65ce8d47b334515d1e1114419a952c7a20fde643e2cb7d7fba90886eb905`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dac8b9094b9d9fb88438fba0a9603978bb1779e919ca8adf8673ef932f74e5`  
		Last Modified: Wed, 24 Feb 2021 21:21:23 GMT  
		Size: 10.9 MB (10925347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114ebf580e52effa6a3b734370fc33000e5a7439f0b0b2b275ffaca7483dd32`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9629cb7ae3d67bb1da05e2a4fa565c7549f1d0df99f27e50987ad0414fa275a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0888c16cdeddffbcaf6f274289f92000cb7e408a60c2788e1cecce57fb4f54d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:33:39 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:33:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:33:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:33:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:33:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:33:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:33:49 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:33:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:33:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:33:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:33:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:33:58 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:33:59 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c560f04d39148af03b91ee7707d8a25136794128fdc0eb1a28ee5a9c7ec5`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 300.4 KB (300351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bb894d60771907a615f58e2c0b5873da52637bf52500990e34621581a232d7`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c61561fb1545eb44bb540b09bf7ce497aa3618f51b8dd8013e161cbe6b595d`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d97783fa5ecc238f39ccba3a47e00bbef6ee3ac8db0ad07989b7f65fac81`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:247ebfeff707410bb47d0a0501aee685d43129a4fab344f361ca1430c28a4058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9eef5ad7357ccba137393d95be15feb69c0fb5bf08d5a63bdd1d15f0a957a92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:19:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:19:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:19:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:19:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:19:32 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:19:37 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:19:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:19:40 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866813d62eb8e73b5cfc9e73e48928d678fcad6123ca0697fdc6ff6faf0c91e`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 300.5 KB (300478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8052626100230d16d27888d060e65aaf770add1ae10f69a8f03a903d274ec2`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6a465134a658869ad61a0ea92cf2775ffd82e4cd1d0e2246f24abd0ac95613`  
		Last Modified: Wed, 24 Feb 2021 21:20:17 GMT  
		Size: 11.3 MB (11272060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fffed8a5a7c6c9efd387b3b851eb42ba3b176b5614156a8f2b5ca6dbfe56e7`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:0fb7ab0f5020028979571375f6603af9a59654678c6e4f03ad921a1393b5c243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:862811186da27cadceb66c7ee0cb45d86e6b602f47863023ed8319b3301dbbd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119510533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24e5592ed0aa110ea96dac4d55eefb729afbdc814df500aa6a787dbc57231e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:37:14 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:37:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:37:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:26:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:28:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:28:28 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:28:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:28:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:28:29 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 22:49:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c21a6730e0112f8caa6cdc154b2f867263b01469a8da8db3b07547c4950a2`  
		Last Modified: Sat, 06 Mar 2021 01:46:38 GMT  
		Size: 280.9 KB (280894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f35c144b30bc90da37f39e5fa735d3ece39f8d810a72e602a654f97c14e28`  
		Last Modified: Sat, 06 Mar 2021 01:46:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d74b5e6c1b32d8da263fffffe1571d0aa7840a360e44cef8824e2f92b6fc711`  
		Last Modified: Thu, 11 Mar 2021 22:33:43 GMT  
		Size: 106.8 MB (106807980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ba6a180f195b6f3ec45af31dc20f7f82de4534fa980b59ffaaf3b77d65165`  
		Last Modified: Thu, 11 Mar 2021 22:33:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4a5846e3583aa5bd3bbad43108ab66cec6cad25f06829e8b10f0d224c15d5`  
		Last Modified: Thu, 11 Mar 2021 22:49:57 GMT  
		Size: 8.3 MB (8310380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8a6abbe5760db7bc9db1db175757935f89f61a0423693ac14c3f91da46abf`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007277fd96ef5c07c805416c73c421afa2999ef84692cbb110e791074063bd12`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c4d0afa340d0e2aa233f8278507aee670023b17b80e590c91d93ef3439de448a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef488fb8def86e1b06487105f395f6fc0a7e087069583f3e431d84bcaae2299`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:02:48 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:05:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:05:39 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:05:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:05:43 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:24:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:24:42 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:24:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:24:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:24:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:24:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:24:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614262833bc8b0fc7ca4f64867b162339accb9d3582c54741d8b49f2c64c09`  
		Last Modified: Thu, 11 Mar 2021 23:08:57 GMT  
		Size: 102.7 MB (102672225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bf2e189cc80b997303b9f227dc8e23de317a042c70a3acca6d8b3788e25aa`  
		Last Modified: Thu, 11 Mar 2021 23:08:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f119c8bfefc5869514223494c22fc23a2d68fc033ee20fedc4b3b174415b76b`  
		Last Modified: Thu, 11 Mar 2021 23:25:39 GMT  
		Size: 7.9 MB (7929405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f4de46b783da3ec5fd21ce4bc46ab92cc63fcdc40618084b1adfc1aba00098`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37870025a40d2ec9d941fcb6204cf69ec8d6772a24b7db7d5db1117781a73d25`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:62667b3a24dd819b71004cb01749b845967c223df5ea625100b41ac3d05e2555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113517439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff54e412af0413f30546b8c74fd8c8be5dbea282237684fb43f71203f2175f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:11:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:13:21 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:13:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:13:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:13:26 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:09 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:10 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:58:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd218a9c9cdf2a32d61b9caeabf05fc557d18aba19567001281413ccc166abb6`  
		Last Modified: Thu, 11 Mar 2021 23:19:59 GMT  
		Size: 102.5 MB (102463603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643306f8eda660cb353e21fe422f75cede99a6c613e960ee2286bc348e8176c`  
		Last Modified: Thu, 11 Mar 2021 23:19:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5f28f428a315bb1f0a9910ebcc1381a83256a56de2e96d61f352ee103e3a9`  
		Last Modified: Thu, 11 Mar 2021 23:59:09 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0a908c65e06d906c5f8352e6430d08d7c9dc1b7dc59a5c291fa66e59aa7e6`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 1.2 MB (1219448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e242abfb42c9c0e708ed52f02bc92c3512595611a1ffcf57ff9cef9d3c394f2`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2082102b6f25fc889876abd33fb7f22883f7bb2e2bce98d8a6034fadb887cf26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ede628fb1a9cfec8f6105c863950f2b5ac5e75252b33cf6a2a05f6bbb57d641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:49:25 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:51:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:51:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:51:27 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:13 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6aafe1b0e31e65c7529ef8d21847b8c1efe056cdcd4fbee6ce827c8a6f80e`  
		Last Modified: Thu, 11 Mar 2021 22:57:06 GMT  
		Size: 102.1 MB (102142762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac1f4721e7976668b36bf40054f4c21e6c868baef018741d21154a99b824f6`  
		Last Modified: Thu, 11 Mar 2021 22:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9845f269e96f38704961fb343cccbba5ce6ff2061a46d2ef294070700edbdd62`  
		Last Modified: Thu, 11 Mar 2021 23:14:19 GMT  
		Size: 8.5 MB (8500022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a957bca51081628082676c05f573ad37667ba4ba87785e3e73197652b7358f`  
		Last Modified: Thu, 11 Mar 2021 23:14:14 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3c4fc1979a993abfec003c90073b87df4264100f18e36620b92953459cde3a`  
		Last Modified: Thu, 11 Mar 2021 23:14:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:83e551e622cb784fb7771f8d614a283626c40214db727d7dea05ac64a8a22966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113984663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d7b1fee3cf2dbef32e9959f80faccc3e466774dbd16ea3ab14918fd6a86609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:22:20 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 12 Mar 2021 00:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:24:30 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:24:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:25:09 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:51:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:51:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:51:55 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:52:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:52:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:52:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:52:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2154d5a1378fc4fbd5545832a4424cc2e5dd3613165269dff45cc20e243032fb`  
		Last Modified: Fri, 12 Mar 2021 00:35:25 GMT  
		Size: 100.8 MB (100802905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57651c1165a6ece6782264b696e85781759407e02c29456a701c0fcd2ee66bec`  
		Last Modified: Fri, 12 Mar 2021 00:35:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf1475a468d7b95375a09ed37f89ee94fee4790a3994ddf52921881a7344172`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 8.9 MB (8921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e317bfdf0439372547a8ace4172d14ae9ec69b87a6aebae08ef2e3399f79d3a`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d267f6d8a55227241eb5b4887182e8235cafdfffe5dff7669c5576540b390cac`  
		Last Modified: Fri, 12 Mar 2021 00:54:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1cc96e1e2875dd10ee3630e1fedf90665895a48e5a75ca4611dfcdf4faaab916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118386946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c72d03c0317c0c4b8c9d6d05ba0f3e4a5389e0d974948f958748fade2ecfa6a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:26:20 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:26:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:26:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:53:49 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:53:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:53:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:53:51 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:46 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ce93a9515faa8483031cd7ac348bce59b30f557f40b533df9e52c358a19e5`  
		Last Modified: Wed, 24 Feb 2021 21:32:29 GMT  
		Size: 281.3 KB (281347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c08039d2964dbc395a13ddd93f041bfb0b0baeae68502ad855f2275c19cdf`  
		Last Modified: Wed, 24 Feb 2021 21:32:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21498377e25a1a2541581a496a9f9201de39caedc60865734db766646a4c8af2`  
		Last Modified: Thu, 11 Mar 2021 22:58:04 GMT  
		Size: 105.9 MB (105920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b19d5e0ba58e1f0c5cf765952f6b60d368718d527771478ca9b28247802316`  
		Last Modified: Thu, 11 Mar 2021 22:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8774f2ce3d2f37a1517d768246eedf3261c9857937f22325c23e630dcab4b`  
		Last Modified: Thu, 11 Mar 2021 23:14:37 GMT  
		Size: 8.4 MB (8352751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c425cbaf74b50e11b534aa5373a068938bf6757dbe03de2347fec50d2c725a`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 1.3 MB (1264422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccdb72140ea082b64ecde8f58d6a55f783edf2f3862bf153e8f985fdb8d9163`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:b479ee29fc292927412fd406cbd98213c86297827a1394d0330aeb893389ca2b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997779833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d39182d3209e4aaf523a2af875e851b8f76036d6c06fb20c6f7fcec6b5513a7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:29:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:33:04 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:33:06 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:06:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:06:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8494855cd5caf3e189463c5ccb6b39747780c1badc12b700373d09d3eda5951`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d01c5a4b0a72580926ec7ca31a0854e4579fc963e0ac611647baf0114f2a66`  
		Last Modified: Thu, 11 Mar 2021 23:45:43 GMT  
		Size: 143.9 MB (143920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50820dad888490de695910927761a6f39cc9279dd81fe9a5c9e6c9251898981a`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dfd1807d2f148f94a7a3347aaf549f9dbc2f2579f0f79923f1f5af98f0b391`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe53f39ec665d626ef91d032f7fd89585e43fc33ccd8683ac6702a9d9e48e2`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5ba9ef95c5e7d8a7b67707b0684405b788b8b40981ecb630f594aa5c2e441`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aff9b53d22053a11e663aac9f51af62d7f29b0f7f6f0796b1bf806f4964f6b`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a037fab4795a44a74e89abfc519243a3cad9ed7e5d5c0109040ff2a2bb457c4`  
		Last Modified: Fri, 12 Mar 2021 00:10:28 GMT  
		Size: 11.5 MB (11517051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f94242e8b9b89dc3a91c2e504dcae074ad187dded384b87b8cf4c29ca92f`  
		Last Modified: Fri, 12 Mar 2021 00:10:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:ab06d627ea66c5536a8cb97a86b3dfed587b811dc803c42dd5fdd65b4255e303
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
$ docker pull caddy@sha256:862811186da27cadceb66c7ee0cb45d86e6b602f47863023ed8319b3301dbbd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119510533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24e5592ed0aa110ea96dac4d55eefb729afbdc814df500aa6a787dbc57231e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:37:14 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:37:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:37:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:26:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:28:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:28:28 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:28:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:28:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:28:29 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 22:49:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c21a6730e0112f8caa6cdc154b2f867263b01469a8da8db3b07547c4950a2`  
		Last Modified: Sat, 06 Mar 2021 01:46:38 GMT  
		Size: 280.9 KB (280894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f35c144b30bc90da37f39e5fa735d3ece39f8d810a72e602a654f97c14e28`  
		Last Modified: Sat, 06 Mar 2021 01:46:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d74b5e6c1b32d8da263fffffe1571d0aa7840a360e44cef8824e2f92b6fc711`  
		Last Modified: Thu, 11 Mar 2021 22:33:43 GMT  
		Size: 106.8 MB (106807980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ba6a180f195b6f3ec45af31dc20f7f82de4534fa980b59ffaaf3b77d65165`  
		Last Modified: Thu, 11 Mar 2021 22:33:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4a5846e3583aa5bd3bbad43108ab66cec6cad25f06829e8b10f0d224c15d5`  
		Last Modified: Thu, 11 Mar 2021 22:49:57 GMT  
		Size: 8.3 MB (8310380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8a6abbe5760db7bc9db1db175757935f89f61a0423693ac14c3f91da46abf`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007277fd96ef5c07c805416c73c421afa2999ef84692cbb110e791074063bd12`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c4d0afa340d0e2aa233f8278507aee670023b17b80e590c91d93ef3439de448a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef488fb8def86e1b06487105f395f6fc0a7e087069583f3e431d84bcaae2299`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:02:48 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:05:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:05:39 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:05:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:05:43 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:24:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:24:42 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:24:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:24:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:24:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:24:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:24:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614262833bc8b0fc7ca4f64867b162339accb9d3582c54741d8b49f2c64c09`  
		Last Modified: Thu, 11 Mar 2021 23:08:57 GMT  
		Size: 102.7 MB (102672225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bf2e189cc80b997303b9f227dc8e23de317a042c70a3acca6d8b3788e25aa`  
		Last Modified: Thu, 11 Mar 2021 23:08:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f119c8bfefc5869514223494c22fc23a2d68fc033ee20fedc4b3b174415b76b`  
		Last Modified: Thu, 11 Mar 2021 23:25:39 GMT  
		Size: 7.9 MB (7929405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f4de46b783da3ec5fd21ce4bc46ab92cc63fcdc40618084b1adfc1aba00098`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37870025a40d2ec9d941fcb6204cf69ec8d6772a24b7db7d5db1117781a73d25`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:62667b3a24dd819b71004cb01749b845967c223df5ea625100b41ac3d05e2555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113517439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff54e412af0413f30546b8c74fd8c8be5dbea282237684fb43f71203f2175f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:11:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:13:21 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:13:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:13:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:13:26 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:09 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:10 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:58:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd218a9c9cdf2a32d61b9caeabf05fc557d18aba19567001281413ccc166abb6`  
		Last Modified: Thu, 11 Mar 2021 23:19:59 GMT  
		Size: 102.5 MB (102463603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643306f8eda660cb353e21fe422f75cede99a6c613e960ee2286bc348e8176c`  
		Last Modified: Thu, 11 Mar 2021 23:19:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5f28f428a315bb1f0a9910ebcc1381a83256a56de2e96d61f352ee103e3a9`  
		Last Modified: Thu, 11 Mar 2021 23:59:09 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0a908c65e06d906c5f8352e6430d08d7c9dc1b7dc59a5c291fa66e59aa7e6`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 1.2 MB (1219448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e242abfb42c9c0e708ed52f02bc92c3512595611a1ffcf57ff9cef9d3c394f2`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2082102b6f25fc889876abd33fb7f22883f7bb2e2bce98d8a6034fadb887cf26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ede628fb1a9cfec8f6105c863950f2b5ac5e75252b33cf6a2a05f6bbb57d641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:49:25 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:51:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:51:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:51:27 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:13 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6aafe1b0e31e65c7529ef8d21847b8c1efe056cdcd4fbee6ce827c8a6f80e`  
		Last Modified: Thu, 11 Mar 2021 22:57:06 GMT  
		Size: 102.1 MB (102142762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac1f4721e7976668b36bf40054f4c21e6c868baef018741d21154a99b824f6`  
		Last Modified: Thu, 11 Mar 2021 22:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9845f269e96f38704961fb343cccbba5ce6ff2061a46d2ef294070700edbdd62`  
		Last Modified: Thu, 11 Mar 2021 23:14:19 GMT  
		Size: 8.5 MB (8500022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a957bca51081628082676c05f573ad37667ba4ba87785e3e73197652b7358f`  
		Last Modified: Thu, 11 Mar 2021 23:14:14 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3c4fc1979a993abfec003c90073b87df4264100f18e36620b92953459cde3a`  
		Last Modified: Thu, 11 Mar 2021 23:14:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:83e551e622cb784fb7771f8d614a283626c40214db727d7dea05ac64a8a22966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113984663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d7b1fee3cf2dbef32e9959f80faccc3e466774dbd16ea3ab14918fd6a86609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:22:20 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 12 Mar 2021 00:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:24:30 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:24:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:25:09 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:51:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:51:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:51:55 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:52:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:52:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:52:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:52:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2154d5a1378fc4fbd5545832a4424cc2e5dd3613165269dff45cc20e243032fb`  
		Last Modified: Fri, 12 Mar 2021 00:35:25 GMT  
		Size: 100.8 MB (100802905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57651c1165a6ece6782264b696e85781759407e02c29456a701c0fcd2ee66bec`  
		Last Modified: Fri, 12 Mar 2021 00:35:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf1475a468d7b95375a09ed37f89ee94fee4790a3994ddf52921881a7344172`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 8.9 MB (8921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e317bfdf0439372547a8ace4172d14ae9ec69b87a6aebae08ef2e3399f79d3a`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d267f6d8a55227241eb5b4887182e8235cafdfffe5dff7669c5576540b390cac`  
		Last Modified: Fri, 12 Mar 2021 00:54:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1cc96e1e2875dd10ee3630e1fedf90665895a48e5a75ca4611dfcdf4faaab916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118386946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c72d03c0317c0c4b8c9d6d05ba0f3e4a5389e0d974948f958748fade2ecfa6a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:26:20 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:26:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:26:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:53:49 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:53:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:53:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:53:51 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:46 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ce93a9515faa8483031cd7ac348bce59b30f557f40b533df9e52c358a19e5`  
		Last Modified: Wed, 24 Feb 2021 21:32:29 GMT  
		Size: 281.3 KB (281347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c08039d2964dbc395a13ddd93f041bfb0b0baeae68502ad855f2275c19cdf`  
		Last Modified: Wed, 24 Feb 2021 21:32:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21498377e25a1a2541581a496a9f9201de39caedc60865734db766646a4c8af2`  
		Last Modified: Thu, 11 Mar 2021 22:58:04 GMT  
		Size: 105.9 MB (105920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b19d5e0ba58e1f0c5cf765952f6b60d368718d527771478ca9b28247802316`  
		Last Modified: Thu, 11 Mar 2021 22:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8774f2ce3d2f37a1517d768246eedf3261c9857937f22325c23e630dcab4b`  
		Last Modified: Thu, 11 Mar 2021 23:14:37 GMT  
		Size: 8.4 MB (8352751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c425cbaf74b50e11b534aa5373a068938bf6757dbe03de2347fec50d2c725a`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 1.3 MB (1264422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccdb72140ea082b64ecde8f58d6a55f783edf2f3862bf153e8f985fdb8d9163`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f51cbb2f6355b4ba86c8133c76ec964e0385fd4a3ee980a35a7e700ebf761366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:0618e3b1bf17154fccafda7e15f9cd3a661e3515ce15e32f578db0fbb8cb4ede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:b479ee29fc292927412fd406cbd98213c86297827a1394d0330aeb893389ca2b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997779833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d39182d3209e4aaf523a2af875e851b8f76036d6c06fb20c6f7fcec6b5513a7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:29:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:33:04 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:33:06 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:06:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:06:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8494855cd5caf3e189463c5ccb6b39747780c1badc12b700373d09d3eda5951`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d01c5a4b0a72580926ec7ca31a0854e4579fc963e0ac611647baf0114f2a66`  
		Last Modified: Thu, 11 Mar 2021 23:45:43 GMT  
		Size: 143.9 MB (143920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50820dad888490de695910927761a6f39cc9279dd81fe9a5c9e6c9251898981a`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dfd1807d2f148f94a7a3347aaf549f9dbc2f2579f0f79923f1f5af98f0b391`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe53f39ec665d626ef91d032f7fd89585e43fc33ccd8683ac6702a9d9e48e2`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5ba9ef95c5e7d8a7b67707b0684405b788b8b40981ecb630f594aa5c2e441`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aff9b53d22053a11e663aac9f51af62d7f29b0f7f6f0796b1bf806f4964f6b`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a037fab4795a44a74e89abfc519243a3cad9ed7e5d5c0109040ff2a2bb457c4`  
		Last Modified: Fri, 12 Mar 2021 00:10:28 GMT  
		Size: 11.5 MB (11517051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f94242e8b9b89dc3a91c2e504dcae074ad187dded384b87b8cf4c29ca92f`  
		Last Modified: Fri, 12 Mar 2021 00:10:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:0d7ec2ae02e36f8374b028af66afcca548c8995638a733f0ad2e7861e2775e7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:dfa33ff752c331d4b76bfe3817fd42ef3ef0bc24d9167cdfdd39f137054ea298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:971ecb6797495e16d5ee3ede15138f5ceaee0930af2ee0b6fbc9dbae848302fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:9485932040de498b47cf0b6cc5d23cbbfd6282e5ff4884b04413cfda0e642661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.3.0` - linux; amd64

```console
$ docker pull caddy@sha256:d0b43ebda8fd47409cec98d5f3c3b4c60bfc6bca35338313c002dc64c2283055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88588539bb905b66ad7f78f35b915f2daf56ec49fd5f20019793e9dbd9747497`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:10:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:10:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:10:52 GMT
ENV CADDY_VERSION=v2.3.0
# Sat, 06 Mar 2021 08:10:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:10:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:10:59 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:10:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296b24b4efd312d2a5e0a24a29635cf8aa098c9c3e50ca6566741a54b2794b`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 300.0 KB (300027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0836949366398b595edf3fde04aff8f2a0c0f4c1ea35372e070f4bf27ce59`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7383a05b49b6f752da622ff9a170dccd483a982060cc06a6be10d6312d32a0`  
		Last Modified: Sat, 06 Mar 2021 08:11:52 GMT  
		Size: 11.6 MB (11622385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701a0726354caf82c1c4be1f558173acf8b6604f7b4118a1097b98424256bd`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c03423186b55d3813eb09d04dc53106635be68cfb5969c12109e08cff9aa2cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569b44d4318ddaf5248442e91df11b525d9ccaf230b7efd78c6ce6ef08281ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:07:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:07:11 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:07:11 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:07:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:07:18 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:07:19 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:07:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:07:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:07:26 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:07:27 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:07:28 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:07:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:07:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9d7c4e3e67f9f36b119476dce4a4951c76aca8f9848b7cc600797ce9a5dbb5`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0438df6797a38cba7f30dd40d58d68e90cf6f6a4ece0a3352142ef610796d1`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1886901d622dcb0b11ff563e6eca542fec29b60ae60c1bf82c8d7271fbcb8`  
		Last Modified: Wed, 24 Feb 2021 21:08:13 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f6d93c8b87b0adc5fdfbfb465ceb4e8c5ccbfe7e75288a0b6247b287bd1d19`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35efa62036c16d5ac4716ce79b11c0505538236542b982ce31e580044712c961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e584e1be15b38bc7eddfd01bedf8038c9b6eb1d20a21df121376bc0878fa2b5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:20:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:20:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:20:25 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:20:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:20:32 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:20:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:20:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:20:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:20:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:20:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:20:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:20:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:20:41 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:20:41 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:20:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38341eca332cf74b9be3ce81ca1d45dfb58d85d6d26b7e95c316e6c9bb29ee72`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 299.2 KB (299205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc65ce8d47b334515d1e1114419a952c7a20fde643e2cb7d7fba90886eb905`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dac8b9094b9d9fb88438fba0a9603978bb1779e919ca8adf8673ef932f74e5`  
		Last Modified: Wed, 24 Feb 2021 21:21:23 GMT  
		Size: 10.9 MB (10925347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114ebf580e52effa6a3b734370fc33000e5a7439f0b0b2b275ffaca7483dd32`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9629cb7ae3d67bb1da05e2a4fa565c7549f1d0df99f27e50987ad0414fa275a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0888c16cdeddffbcaf6f274289f92000cb7e408a60c2788e1cecce57fb4f54d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:33:39 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:33:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:33:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:33:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:33:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:33:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:33:49 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:33:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:33:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:33:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:33:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:33:58 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:33:59 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c560f04d39148af03b91ee7707d8a25136794128fdc0eb1a28ee5a9c7ec5`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 300.4 KB (300351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bb894d60771907a615f58e2c0b5873da52637bf52500990e34621581a232d7`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c61561fb1545eb44bb540b09bf7ce497aa3618f51b8dd8013e161cbe6b595d`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d97783fa5ecc238f39ccba3a47e00bbef6ee3ac8db0ad07989b7f65fac81`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; s390x

```console
$ docker pull caddy@sha256:247ebfeff707410bb47d0a0501aee685d43129a4fab344f361ca1430c28a4058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9eef5ad7357ccba137393d95be15feb69c0fb5bf08d5a63bdd1d15f0a957a92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:19:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:19:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:19:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:19:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:19:32 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:19:37 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:19:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:19:40 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866813d62eb8e73b5cfc9e73e48928d678fcad6123ca0697fdc6ff6faf0c91e`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 300.5 KB (300478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8052626100230d16d27888d060e65aaf770add1ae10f69a8f03a903d274ec2`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6a465134a658869ad61a0ea92cf2775ffd82e4cd1d0e2246f24abd0ac95613`  
		Last Modified: Wed, 24 Feb 2021 21:20:17 GMT  
		Size: 11.3 MB (11272060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fffed8a5a7c6c9efd387b3b851eb42ba3b176b5614156a8f2b5ca6dbfe56e7`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-alpine`

```console
$ docker pull caddy@sha256:30cf6a3da8365c2d9344adfc42b33a5b6e01dc4943c75b0132d556d12bd5f995
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
$ docker pull caddy@sha256:d0b43ebda8fd47409cec98d5f3c3b4c60bfc6bca35338313c002dc64c2283055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88588539bb905b66ad7f78f35b915f2daf56ec49fd5f20019793e9dbd9747497`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:10:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:10:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:10:52 GMT
ENV CADDY_VERSION=v2.3.0
# Sat, 06 Mar 2021 08:10:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:10:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:10:59 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:10:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296b24b4efd312d2a5e0a24a29635cf8aa098c9c3e50ca6566741a54b2794b`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 300.0 KB (300027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0836949366398b595edf3fde04aff8f2a0c0f4c1ea35372e070f4bf27ce59`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7383a05b49b6f752da622ff9a170dccd483a982060cc06a6be10d6312d32a0`  
		Last Modified: Sat, 06 Mar 2021 08:11:52 GMT  
		Size: 11.6 MB (11622385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701a0726354caf82c1c4be1f558173acf8b6604f7b4118a1097b98424256bd`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c03423186b55d3813eb09d04dc53106635be68cfb5969c12109e08cff9aa2cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569b44d4318ddaf5248442e91df11b525d9ccaf230b7efd78c6ce6ef08281ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:07:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:07:11 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:07:11 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:07:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:07:18 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:07:19 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:07:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:07:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:07:26 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:07:27 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:07:28 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:07:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:07:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9d7c4e3e67f9f36b119476dce4a4951c76aca8f9848b7cc600797ce9a5dbb5`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0438df6797a38cba7f30dd40d58d68e90cf6f6a4ece0a3352142ef610796d1`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1886901d622dcb0b11ff563e6eca542fec29b60ae60c1bf82c8d7271fbcb8`  
		Last Modified: Wed, 24 Feb 2021 21:08:13 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f6d93c8b87b0adc5fdfbfb465ceb4e8c5ccbfe7e75288a0b6247b287bd1d19`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35efa62036c16d5ac4716ce79b11c0505538236542b982ce31e580044712c961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e584e1be15b38bc7eddfd01bedf8038c9b6eb1d20a21df121376bc0878fa2b5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:20:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:20:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:20:25 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:20:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:20:32 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:20:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:20:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:20:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:20:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:20:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:20:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:20:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:20:41 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:20:41 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:20:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38341eca332cf74b9be3ce81ca1d45dfb58d85d6d26b7e95c316e6c9bb29ee72`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 299.2 KB (299205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc65ce8d47b334515d1e1114419a952c7a20fde643e2cb7d7fba90886eb905`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dac8b9094b9d9fb88438fba0a9603978bb1779e919ca8adf8673ef932f74e5`  
		Last Modified: Wed, 24 Feb 2021 21:21:23 GMT  
		Size: 10.9 MB (10925347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114ebf580e52effa6a3b734370fc33000e5a7439f0b0b2b275ffaca7483dd32`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9629cb7ae3d67bb1da05e2a4fa565c7549f1d0df99f27e50987ad0414fa275a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0888c16cdeddffbcaf6f274289f92000cb7e408a60c2788e1cecce57fb4f54d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:33:39 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:33:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:33:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:33:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:33:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:33:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:33:49 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:33:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:33:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:33:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:33:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:33:58 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:33:59 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c560f04d39148af03b91ee7707d8a25136794128fdc0eb1a28ee5a9c7ec5`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 300.4 KB (300351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bb894d60771907a615f58e2c0b5873da52637bf52500990e34621581a232d7`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c61561fb1545eb44bb540b09bf7ce497aa3618f51b8dd8013e161cbe6b595d`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d97783fa5ecc238f39ccba3a47e00bbef6ee3ac8db0ad07989b7f65fac81`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:247ebfeff707410bb47d0a0501aee685d43129a4fab344f361ca1430c28a4058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9eef5ad7357ccba137393d95be15feb69c0fb5bf08d5a63bdd1d15f0a957a92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:19:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:19:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:19:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:19:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:19:32 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:19:37 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:19:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:19:40 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866813d62eb8e73b5cfc9e73e48928d678fcad6123ca0697fdc6ff6faf0c91e`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 300.5 KB (300478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8052626100230d16d27888d060e65aaf770add1ae10f69a8f03a903d274ec2`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6a465134a658869ad61a0ea92cf2775ffd82e4cd1d0e2246f24abd0ac95613`  
		Last Modified: Wed, 24 Feb 2021 21:20:17 GMT  
		Size: 11.3 MB (11272060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fffed8a5a7c6c9efd387b3b851eb42ba3b176b5614156a8f2b5ca6dbfe56e7`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder`

```console
$ docker pull caddy@sha256:0fb7ab0f5020028979571375f6603af9a59654678c6e4f03ad921a1393b5c243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.3.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:862811186da27cadceb66c7ee0cb45d86e6b602f47863023ed8319b3301dbbd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119510533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24e5592ed0aa110ea96dac4d55eefb729afbdc814df500aa6a787dbc57231e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:37:14 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:37:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:37:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:26:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:28:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:28:28 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:28:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:28:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:28:29 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 22:49:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c21a6730e0112f8caa6cdc154b2f867263b01469a8da8db3b07547c4950a2`  
		Last Modified: Sat, 06 Mar 2021 01:46:38 GMT  
		Size: 280.9 KB (280894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f35c144b30bc90da37f39e5fa735d3ece39f8d810a72e602a654f97c14e28`  
		Last Modified: Sat, 06 Mar 2021 01:46:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d74b5e6c1b32d8da263fffffe1571d0aa7840a360e44cef8824e2f92b6fc711`  
		Last Modified: Thu, 11 Mar 2021 22:33:43 GMT  
		Size: 106.8 MB (106807980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ba6a180f195b6f3ec45af31dc20f7f82de4534fa980b59ffaaf3b77d65165`  
		Last Modified: Thu, 11 Mar 2021 22:33:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4a5846e3583aa5bd3bbad43108ab66cec6cad25f06829e8b10f0d224c15d5`  
		Last Modified: Thu, 11 Mar 2021 22:49:57 GMT  
		Size: 8.3 MB (8310380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8a6abbe5760db7bc9db1db175757935f89f61a0423693ac14c3f91da46abf`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007277fd96ef5c07c805416c73c421afa2999ef84692cbb110e791074063bd12`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c4d0afa340d0e2aa233f8278507aee670023b17b80e590c91d93ef3439de448a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef488fb8def86e1b06487105f395f6fc0a7e087069583f3e431d84bcaae2299`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:02:48 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:05:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:05:39 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:05:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:05:43 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:24:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:24:42 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:24:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:24:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:24:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:24:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:24:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614262833bc8b0fc7ca4f64867b162339accb9d3582c54741d8b49f2c64c09`  
		Last Modified: Thu, 11 Mar 2021 23:08:57 GMT  
		Size: 102.7 MB (102672225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bf2e189cc80b997303b9f227dc8e23de317a042c70a3acca6d8b3788e25aa`  
		Last Modified: Thu, 11 Mar 2021 23:08:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f119c8bfefc5869514223494c22fc23a2d68fc033ee20fedc4b3b174415b76b`  
		Last Modified: Thu, 11 Mar 2021 23:25:39 GMT  
		Size: 7.9 MB (7929405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f4de46b783da3ec5fd21ce4bc46ab92cc63fcdc40618084b1adfc1aba00098`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37870025a40d2ec9d941fcb6204cf69ec8d6772a24b7db7d5db1117781a73d25`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:62667b3a24dd819b71004cb01749b845967c223df5ea625100b41ac3d05e2555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113517439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff54e412af0413f30546b8c74fd8c8be5dbea282237684fb43f71203f2175f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:11:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:13:21 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:13:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:13:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:13:26 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:09 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:10 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:58:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd218a9c9cdf2a32d61b9caeabf05fc557d18aba19567001281413ccc166abb6`  
		Last Modified: Thu, 11 Mar 2021 23:19:59 GMT  
		Size: 102.5 MB (102463603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643306f8eda660cb353e21fe422f75cede99a6c613e960ee2286bc348e8176c`  
		Last Modified: Thu, 11 Mar 2021 23:19:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5f28f428a315bb1f0a9910ebcc1381a83256a56de2e96d61f352ee103e3a9`  
		Last Modified: Thu, 11 Mar 2021 23:59:09 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0a908c65e06d906c5f8352e6430d08d7c9dc1b7dc59a5c291fa66e59aa7e6`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 1.2 MB (1219448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e242abfb42c9c0e708ed52f02bc92c3512595611a1ffcf57ff9cef9d3c394f2`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2082102b6f25fc889876abd33fb7f22883f7bb2e2bce98d8a6034fadb887cf26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ede628fb1a9cfec8f6105c863950f2b5ac5e75252b33cf6a2a05f6bbb57d641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:49:25 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:51:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:51:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:51:27 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:13 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6aafe1b0e31e65c7529ef8d21847b8c1efe056cdcd4fbee6ce827c8a6f80e`  
		Last Modified: Thu, 11 Mar 2021 22:57:06 GMT  
		Size: 102.1 MB (102142762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac1f4721e7976668b36bf40054f4c21e6c868baef018741d21154a99b824f6`  
		Last Modified: Thu, 11 Mar 2021 22:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9845f269e96f38704961fb343cccbba5ce6ff2061a46d2ef294070700edbdd62`  
		Last Modified: Thu, 11 Mar 2021 23:14:19 GMT  
		Size: 8.5 MB (8500022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a957bca51081628082676c05f573ad37667ba4ba87785e3e73197652b7358f`  
		Last Modified: Thu, 11 Mar 2021 23:14:14 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3c4fc1979a993abfec003c90073b87df4264100f18e36620b92953459cde3a`  
		Last Modified: Thu, 11 Mar 2021 23:14:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:83e551e622cb784fb7771f8d614a283626c40214db727d7dea05ac64a8a22966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113984663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d7b1fee3cf2dbef32e9959f80faccc3e466774dbd16ea3ab14918fd6a86609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:22:20 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 12 Mar 2021 00:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:24:30 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:24:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:25:09 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:51:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:51:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:51:55 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:52:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:52:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:52:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:52:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2154d5a1378fc4fbd5545832a4424cc2e5dd3613165269dff45cc20e243032fb`  
		Last Modified: Fri, 12 Mar 2021 00:35:25 GMT  
		Size: 100.8 MB (100802905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57651c1165a6ece6782264b696e85781759407e02c29456a701c0fcd2ee66bec`  
		Last Modified: Fri, 12 Mar 2021 00:35:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf1475a468d7b95375a09ed37f89ee94fee4790a3994ddf52921881a7344172`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 8.9 MB (8921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e317bfdf0439372547a8ace4172d14ae9ec69b87a6aebae08ef2e3399f79d3a`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d267f6d8a55227241eb5b4887182e8235cafdfffe5dff7669c5576540b390cac`  
		Last Modified: Fri, 12 Mar 2021 00:54:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1cc96e1e2875dd10ee3630e1fedf90665895a48e5a75ca4611dfcdf4faaab916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118386946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c72d03c0317c0c4b8c9d6d05ba0f3e4a5389e0d974948f958748fade2ecfa6a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:26:20 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:26:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:26:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:53:49 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:53:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:53:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:53:51 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:46 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ce93a9515faa8483031cd7ac348bce59b30f557f40b533df9e52c358a19e5`  
		Last Modified: Wed, 24 Feb 2021 21:32:29 GMT  
		Size: 281.3 KB (281347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c08039d2964dbc395a13ddd93f041bfb0b0baeae68502ad855f2275c19cdf`  
		Last Modified: Wed, 24 Feb 2021 21:32:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21498377e25a1a2541581a496a9f9201de39caedc60865734db766646a4c8af2`  
		Last Modified: Thu, 11 Mar 2021 22:58:04 GMT  
		Size: 105.9 MB (105920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b19d5e0ba58e1f0c5cf765952f6b60d368718d527771478ca9b28247802316`  
		Last Modified: Thu, 11 Mar 2021 22:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8774f2ce3d2f37a1517d768246eedf3261c9857937f22325c23e630dcab4b`  
		Last Modified: Thu, 11 Mar 2021 23:14:37 GMT  
		Size: 8.4 MB (8352751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c425cbaf74b50e11b534aa5373a068938bf6757dbe03de2347fec50d2c725a`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 1.3 MB (1264422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccdb72140ea082b64ecde8f58d6a55f783edf2f3862bf153e8f985fdb8d9163`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:b479ee29fc292927412fd406cbd98213c86297827a1394d0330aeb893389ca2b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997779833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d39182d3209e4aaf523a2af875e851b8f76036d6c06fb20c6f7fcec6b5513a7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:29:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:33:04 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:33:06 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:06:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:06:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8494855cd5caf3e189463c5ccb6b39747780c1badc12b700373d09d3eda5951`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d01c5a4b0a72580926ec7ca31a0854e4579fc963e0ac611647baf0114f2a66`  
		Last Modified: Thu, 11 Mar 2021 23:45:43 GMT  
		Size: 143.9 MB (143920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50820dad888490de695910927761a6f39cc9279dd81fe9a5c9e6c9251898981a`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dfd1807d2f148f94a7a3347aaf549f9dbc2f2579f0f79923f1f5af98f0b391`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe53f39ec665d626ef91d032f7fd89585e43fc33ccd8683ac6702a9d9e48e2`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5ba9ef95c5e7d8a7b67707b0684405b788b8b40981ecb630f594aa5c2e441`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aff9b53d22053a11e663aac9f51af62d7f29b0f7f6f0796b1bf806f4964f6b`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a037fab4795a44a74e89abfc519243a3cad9ed7e5d5c0109040ff2a2bb457c4`  
		Last Modified: Fri, 12 Mar 2021 00:10:28 GMT  
		Size: 11.5 MB (11517051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f94242e8b9b89dc3a91c2e504dcae074ad187dded384b87b8cf4c29ca92f`  
		Last Modified: Fri, 12 Mar 2021 00:10:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:ab06d627ea66c5536a8cb97a86b3dfed587b811dc803c42dd5fdd65b4255e303
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
$ docker pull caddy@sha256:862811186da27cadceb66c7ee0cb45d86e6b602f47863023ed8319b3301dbbd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119510533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24e5592ed0aa110ea96dac4d55eefb729afbdc814df500aa6a787dbc57231e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:37:14 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:37:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:37:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:26:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:28:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:28:28 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:28:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:28:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:28:29 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 22:49:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c21a6730e0112f8caa6cdc154b2f867263b01469a8da8db3b07547c4950a2`  
		Last Modified: Sat, 06 Mar 2021 01:46:38 GMT  
		Size: 280.9 KB (280894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f35c144b30bc90da37f39e5fa735d3ece39f8d810a72e602a654f97c14e28`  
		Last Modified: Sat, 06 Mar 2021 01:46:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d74b5e6c1b32d8da263fffffe1571d0aa7840a360e44cef8824e2f92b6fc711`  
		Last Modified: Thu, 11 Mar 2021 22:33:43 GMT  
		Size: 106.8 MB (106807980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ba6a180f195b6f3ec45af31dc20f7f82de4534fa980b59ffaaf3b77d65165`  
		Last Modified: Thu, 11 Mar 2021 22:33:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4a5846e3583aa5bd3bbad43108ab66cec6cad25f06829e8b10f0d224c15d5`  
		Last Modified: Thu, 11 Mar 2021 22:49:57 GMT  
		Size: 8.3 MB (8310380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8a6abbe5760db7bc9db1db175757935f89f61a0423693ac14c3f91da46abf`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007277fd96ef5c07c805416c73c421afa2999ef84692cbb110e791074063bd12`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c4d0afa340d0e2aa233f8278507aee670023b17b80e590c91d93ef3439de448a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef488fb8def86e1b06487105f395f6fc0a7e087069583f3e431d84bcaae2299`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:02:48 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:05:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:05:39 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:05:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:05:43 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:24:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:24:42 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:24:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:24:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:24:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:24:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:24:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614262833bc8b0fc7ca4f64867b162339accb9d3582c54741d8b49f2c64c09`  
		Last Modified: Thu, 11 Mar 2021 23:08:57 GMT  
		Size: 102.7 MB (102672225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bf2e189cc80b997303b9f227dc8e23de317a042c70a3acca6d8b3788e25aa`  
		Last Modified: Thu, 11 Mar 2021 23:08:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f119c8bfefc5869514223494c22fc23a2d68fc033ee20fedc4b3b174415b76b`  
		Last Modified: Thu, 11 Mar 2021 23:25:39 GMT  
		Size: 7.9 MB (7929405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f4de46b783da3ec5fd21ce4bc46ab92cc63fcdc40618084b1adfc1aba00098`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37870025a40d2ec9d941fcb6204cf69ec8d6772a24b7db7d5db1117781a73d25`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:62667b3a24dd819b71004cb01749b845967c223df5ea625100b41ac3d05e2555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113517439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff54e412af0413f30546b8c74fd8c8be5dbea282237684fb43f71203f2175f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:11:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:13:21 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:13:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:13:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:13:26 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:09 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:10 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:58:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd218a9c9cdf2a32d61b9caeabf05fc557d18aba19567001281413ccc166abb6`  
		Last Modified: Thu, 11 Mar 2021 23:19:59 GMT  
		Size: 102.5 MB (102463603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643306f8eda660cb353e21fe422f75cede99a6c613e960ee2286bc348e8176c`  
		Last Modified: Thu, 11 Mar 2021 23:19:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5f28f428a315bb1f0a9910ebcc1381a83256a56de2e96d61f352ee103e3a9`  
		Last Modified: Thu, 11 Mar 2021 23:59:09 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0a908c65e06d906c5f8352e6430d08d7c9dc1b7dc59a5c291fa66e59aa7e6`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 1.2 MB (1219448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e242abfb42c9c0e708ed52f02bc92c3512595611a1ffcf57ff9cef9d3c394f2`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2082102b6f25fc889876abd33fb7f22883f7bb2e2bce98d8a6034fadb887cf26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ede628fb1a9cfec8f6105c863950f2b5ac5e75252b33cf6a2a05f6bbb57d641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:49:25 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:51:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:51:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:51:27 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:13 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6aafe1b0e31e65c7529ef8d21847b8c1efe056cdcd4fbee6ce827c8a6f80e`  
		Last Modified: Thu, 11 Mar 2021 22:57:06 GMT  
		Size: 102.1 MB (102142762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac1f4721e7976668b36bf40054f4c21e6c868baef018741d21154a99b824f6`  
		Last Modified: Thu, 11 Mar 2021 22:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9845f269e96f38704961fb343cccbba5ce6ff2061a46d2ef294070700edbdd62`  
		Last Modified: Thu, 11 Mar 2021 23:14:19 GMT  
		Size: 8.5 MB (8500022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a957bca51081628082676c05f573ad37667ba4ba87785e3e73197652b7358f`  
		Last Modified: Thu, 11 Mar 2021 23:14:14 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3c4fc1979a993abfec003c90073b87df4264100f18e36620b92953459cde3a`  
		Last Modified: Thu, 11 Mar 2021 23:14:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:83e551e622cb784fb7771f8d614a283626c40214db727d7dea05ac64a8a22966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113984663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d7b1fee3cf2dbef32e9959f80faccc3e466774dbd16ea3ab14918fd6a86609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:22:20 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 12 Mar 2021 00:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:24:30 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:24:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:25:09 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:51:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:51:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:51:55 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:52:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:52:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:52:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:52:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2154d5a1378fc4fbd5545832a4424cc2e5dd3613165269dff45cc20e243032fb`  
		Last Modified: Fri, 12 Mar 2021 00:35:25 GMT  
		Size: 100.8 MB (100802905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57651c1165a6ece6782264b696e85781759407e02c29456a701c0fcd2ee66bec`  
		Last Modified: Fri, 12 Mar 2021 00:35:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf1475a468d7b95375a09ed37f89ee94fee4790a3994ddf52921881a7344172`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 8.9 MB (8921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e317bfdf0439372547a8ace4172d14ae9ec69b87a6aebae08ef2e3399f79d3a`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d267f6d8a55227241eb5b4887182e8235cafdfffe5dff7669c5576540b390cac`  
		Last Modified: Fri, 12 Mar 2021 00:54:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1cc96e1e2875dd10ee3630e1fedf90665895a48e5a75ca4611dfcdf4faaab916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118386946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c72d03c0317c0c4b8c9d6d05ba0f3e4a5389e0d974948f958748fade2ecfa6a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:26:20 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:26:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:26:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:53:49 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:53:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:53:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:53:51 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:46 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ce93a9515faa8483031cd7ac348bce59b30f557f40b533df9e52c358a19e5`  
		Last Modified: Wed, 24 Feb 2021 21:32:29 GMT  
		Size: 281.3 KB (281347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c08039d2964dbc395a13ddd93f041bfb0b0baeae68502ad855f2275c19cdf`  
		Last Modified: Wed, 24 Feb 2021 21:32:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21498377e25a1a2541581a496a9f9201de39caedc60865734db766646a4c8af2`  
		Last Modified: Thu, 11 Mar 2021 22:58:04 GMT  
		Size: 105.9 MB (105920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b19d5e0ba58e1f0c5cf765952f6b60d368718d527771478ca9b28247802316`  
		Last Modified: Thu, 11 Mar 2021 22:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8774f2ce3d2f37a1517d768246eedf3261c9857937f22325c23e630dcab4b`  
		Last Modified: Thu, 11 Mar 2021 23:14:37 GMT  
		Size: 8.4 MB (8352751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c425cbaf74b50e11b534aa5373a068938bf6757dbe03de2347fec50d2c725a`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 1.3 MB (1264422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccdb72140ea082b64ecde8f58d6a55f783edf2f3862bf153e8f985fdb8d9163`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f51cbb2f6355b4ba86c8133c76ec964e0385fd4a3ee980a35a7e700ebf761366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:0618e3b1bf17154fccafda7e15f9cd3a661e3515ce15e32f578db0fbb8cb4ede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:b479ee29fc292927412fd406cbd98213c86297827a1394d0330aeb893389ca2b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997779833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d39182d3209e4aaf523a2af875e851b8f76036d6c06fb20c6f7fcec6b5513a7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:29:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:33:04 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:33:06 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:06:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:06:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8494855cd5caf3e189463c5ccb6b39747780c1badc12b700373d09d3eda5951`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d01c5a4b0a72580926ec7ca31a0854e4579fc963e0ac611647baf0114f2a66`  
		Last Modified: Thu, 11 Mar 2021 23:45:43 GMT  
		Size: 143.9 MB (143920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50820dad888490de695910927761a6f39cc9279dd81fe9a5c9e6c9251898981a`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dfd1807d2f148f94a7a3347aaf549f9dbc2f2579f0f79923f1f5af98f0b391`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe53f39ec665d626ef91d032f7fd89585e43fc33ccd8683ac6702a9d9e48e2`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5ba9ef95c5e7d8a7b67707b0684405b788b8b40981ecb630f594aa5c2e441`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aff9b53d22053a11e663aac9f51af62d7f29b0f7f6f0796b1bf806f4964f6b`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a037fab4795a44a74e89abfc519243a3cad9ed7e5d5c0109040ff2a2bb457c4`  
		Last Modified: Fri, 12 Mar 2021 00:10:28 GMT  
		Size: 11.5 MB (11517051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f94242e8b9b89dc3a91c2e504dcae074ad187dded384b87b8cf4c29ca92f`  
		Last Modified: Fri, 12 Mar 2021 00:10:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore`

```console
$ docker pull caddy@sha256:0d7ec2ae02e36f8374b028af66afcca548c8995638a733f0ad2e7861e2775e7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.3.0-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:dfa33ff752c331d4b76bfe3817fd42ef3ef0bc24d9167cdfdd39f137054ea298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.3.0-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:971ecb6797495e16d5ee3ede15138f5ceaee0930af2ee0b6fbc9dbae848302fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1`

```console
$ docker pull caddy@sha256:f5682923012bd0457cb2a67a4847e322d9bd7e20deae04a36084b26361ce7cda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.1` - linux; amd64

```console
$ docker pull caddy@sha256:292728877c3fc821295b18467bead2be953dd9b0f0d460eeeffd6b6ba357ab4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14763931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1116ab784c1c43b47dc886cedb417f7c56de689bb60adc895f4538d10da87cc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:11:13 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:11:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:11:14 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Sat, 06 Mar 2021 08:11:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:11:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:11:18 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:11:18 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:11:18 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:11:18 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:11:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:11:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:11:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:11:20 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:11:20 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:11:21 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:11:21 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:11:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5621b554e24c44d7f631f7f0d4697255d447db5706e62161700d99a967e772c0`  
		Last Modified: Sat, 06 Mar 2021 08:12:20 GMT  
		Size: 300.4 KB (300402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b5cc7d40fe5b30ae3330852ebd414b71cec7693439fa8ea967cceb1d417ce`  
		Last Modified: Sat, 06 Mar 2021 08:12:20 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e541183feba6e676730c42880d65c075b0b7905af7dbfe0d55009667a9619145`  
		Last Modified: Sat, 06 Mar 2021 08:12:23 GMT  
		Size: 11.6 MB (11645890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f70013118953696dc59d068edba771a221bac2000df2f75cae9e2c989e1e09`  
		Last Modified: Sat, 06 Mar 2021 08:12:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:69ed026d4046988c7cfdb7d092d38b051af05f515c2c582640359a3b320a19fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13898470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5128877c7baed77cfb7dc037f11121a9aec61949f983428060720076eddc3e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:49:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:49:59 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:49:59 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:50:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:50:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:50:07 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:50:08 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:50:09 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:50:10 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:50:11 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:50:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:50:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:50:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:50:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:50:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:50:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:50:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:50:19 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:50:20 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:50:21 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:50:23 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:50:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435d76e6be3eef1e1ee27e127fafe5a99f442a92a7467b0866c4fb65ba4113b`  
		Last Modified: Wed, 24 Feb 2021 18:51:20 GMT  
		Size: 300.5 KB (300516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed97964c38308666a2f1211f6a5cfb26159b76e7d37a3eb8a4928989c8f862`  
		Last Modified: Wed, 24 Feb 2021 18:51:21 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e773a4b13e9da28035f76451153afcdec1f2497b19749b811b7877ce7135779c`  
		Last Modified: Wed, 24 Feb 2021 18:51:24 GMT  
		Size: 11.0 MB (10969934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94dd2f7265c37d9eadfc580dec6754dfa426f11cb141b8ddbc8c5b2dc5a7681`  
		Last Modified: Wed, 24 Feb 2021 18:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:504dc03b283ba138bea4b2d69113a4d751d8c276f07a6b704cc4866fe57e424b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13677502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce15e29dded4c237de13a06d5c8681e93e97b392f9474dcef8630fc3f2b3a8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:58:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:58:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:58:08 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:58:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:58:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:58:15 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:58:16 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:58:16 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:58:17 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:58:19 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:58:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:58:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:58:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:58:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:58:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:58:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:58:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:58:25 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:58:26 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:58:27 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:58:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:58:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57f6854a8c929241451c6d527ac6efdee08455ee8c27aed146be03c5ad806a`  
		Last Modified: Wed, 24 Feb 2021 18:59:25 GMT  
		Size: 299.7 KB (299665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52063aab834f7e32087615a6698bd11bcc3ade3eb55687eac04d726ab9beeb04`  
		Last Modified: Wed, 24 Feb 2021 18:59:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fbdd64ea7052537bb15fdf9afa804352448372aeef61c0fcdc27a4fce971d7`  
		Last Modified: Wed, 24 Feb 2021 18:59:29 GMT  
		Size: 10.9 MB (10947961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515983999c4dfe73c741f123ff20ea42405a945d46673dd1bfe2695c464b32bf`  
		Last Modified: Wed, 24 Feb 2021 18:59:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5e6321e0c3df5fdb54f8771ed7ecd084831c7bb1dcf89ff3bba906bb6c10280a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13643152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44faf6dde77510e96fd734df5810f321b01a0630c7fc25b94bc2ddd6fc7b980`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:48:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:48:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:48:05 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:48:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:48:11 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:48:12 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:48:12 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:48:13 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:48:14 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:48:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:48:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:48:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:48:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:48:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:48:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:48:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:48:19 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:48:20 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:48:21 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:48:22 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:48:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677d00efd0cb981b2b1ec36a240fce8a89ec062c22e82f307dc6d2651ba6563`  
		Last Modified: Wed, 24 Feb 2021 18:49:19 GMT  
		Size: 300.6 KB (300624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1840450bb57f5fddd099628bb8f9fd57e0b070b11c7f6156e3206be7ce97dae`  
		Last Modified: Wed, 24 Feb 2021 18:49:19 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5716ac42e1610a59f8df7b7f4c4c2a62e28f4a325b0ce932624885fda5acc450`  
		Last Modified: Wed, 24 Feb 2021 18:49:22 GMT  
		Size: 10.6 MB (10624970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bf56fedcfd9886bf3d4adadd089babeb8ba22acec7bd4e7a56382595ef6aa9`  
		Last Modified: Wed, 24 Feb 2021 18:49:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:1bf3b5016c63ee5734915f350b9e29553419eeaf5fe24c1ccbe2daac07606465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13387481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25b9219d7eaa3e483ca62e74df67b8b41b392979867c8588cbd9ddcee0e0771`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 19:53:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 19:54:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 19:54:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:54:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 19:54:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 19:54:30 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 19:54:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 19:54:38 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 19:54:44 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 19:54:53 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:55:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:55:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:55:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:55:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:55:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:55:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:55:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:55:36 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:55:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:55:44 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:55:51 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 19:55:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbd40a596b750ffbee0cd1cf44fbaee64a6e8aff893818fd8de97c75ab7d420`  
		Last Modified: Wed, 24 Feb 2021 19:58:09 GMT  
		Size: 302.5 KB (302524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829bd2a32cf8c0482e15697e74af7944b770aa08730dfb0a976ac07db2290d6a`  
		Last Modified: Wed, 24 Feb 2021 19:58:09 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74c34fc68a5ade6104fdc66c39bc89fa91b5169d51d4ad8e6c5c793bfa450db`  
		Last Modified: Wed, 24 Feb 2021 19:58:11 GMT  
		Size: 10.3 MB (10265885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dee8547b806efa1a0876f5c3fcb41f5f5e5374df0602acc3a31d49892bbeb3`  
		Last Modified: Wed, 24 Feb 2021 19:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; s390x

```console
$ docker pull caddy@sha256:0c9cd2a968cf969ece10e66e605defb77deb94024fa4c713e6ad63cfd7ec8762
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14199778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fcb091c13bf8102a1e374393ddeebc38c4096b89dbaed3a48c3aa723f7f336f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:41:27 GMT
ADD file:630c66f8d774d75b51e32aff812b438d377ebd3389c4aa6c324fdf8c03b6fa13 in / 
# Wed, 17 Feb 2021 20:41:27 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:41:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:41:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:41:51 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:42:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:42:00 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:42:00 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:42:01 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:42:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:42:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:42:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:42:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:42:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:42:06 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:42:07 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:42:07 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:42:08 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:42:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ff5e8cb87555e9fa38a441f5cf0414e91353e2cd21cdb48d48b7de5bb39ce674`  
		Last Modified: Wed, 17 Feb 2021 20:41:58 GMT  
		Size: 2.6 MB (2602381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3fdfa6c58844c6cc4a07b66ee1ef0a17f8699df726982b254ff58a2117abd1`  
		Last Modified: Wed, 24 Feb 2021 18:42:52 GMT  
		Size: 300.8 KB (300837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bdb77fb831f3e597bfccda2296099260d12b7e671c7697a6f722c1af54f650`  
		Last Modified: Wed, 24 Feb 2021 18:42:53 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c299797220d87efdd996a17402dcd1e747734ac17c3f524fcdb8d5a0b4f4cccd`  
		Last Modified: Wed, 24 Feb 2021 18:42:59 GMT  
		Size: 11.3 MB (11290578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1c503c26851e352a5fe95cb24e8a73b2a5d10539ea54d80325f801441190de`  
		Last Modified: Wed, 24 Feb 2021 18:42:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:6e5d5fea5cb01c12f4a392581b1d7cd9c8d057edf35421f107831ac987426788
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487833197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d9298e9342ee167543a1f5ea16eb3acde3c3e78c807d7d27b76ed6bc7587f9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:35:55 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:36:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:36:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:36:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:36:29 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:36:31 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:36:32 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:36:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:36:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:36:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:36:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:36:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:36:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:36:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:36:40 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:36:41 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:36:42 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:37:01 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:37:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc803029bd3ef109ba5043ff19061940f4d933b3b12efaadce4d958fff6984b`  
		Last Modified: Wed, 10 Mar 2021 21:45:26 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e23f022464526cb08cf5ae2524d4194aeb092d552b2a12309a02e731b92f2d`  
		Last Modified: Wed, 10 Mar 2021 21:45:30 GMT  
		Size: 16.5 MB (16480793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4417b70d9203a0f38da3e90189d96fca91c20a89c9f840dc3bf64b4f2561ae5c`  
		Last Modified: Wed, 10 Mar 2021 21:45:26 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4755067618a3cdc748f363c5f1a3da8eef0324233e5927f7dbac370b44bdc0`  
		Last Modified: Wed, 10 Mar 2021 21:45:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a4666bc7b476eb9b14bea25d19716eabf278bcba06df2e012e67a38477aa6`  
		Last Modified: Wed, 10 Mar 2021 21:45:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1c2bc1c49e7b0cba9e9ca161fc75374d674e2149ea25c38cf3ceeb9ce2cd5c`  
		Last Modified: Wed, 10 Mar 2021 21:45:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8c6b745994cb1e2bf9dcd0d2819313119ebc53c3fe9b49cdae27bad55cd4ab`  
		Last Modified: Wed, 10 Mar 2021 21:45:23 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0539021a8993cee20a823ee8225ec8615125fa5e331639602e11912f8a3e03c2`  
		Last Modified: Wed, 10 Mar 2021 21:45:24 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dbc014cc64499a05b9a2c7672e407fcf64a2c92e931fb4459f0a576d56d5fd`  
		Last Modified: Wed, 10 Mar 2021 21:45:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1bd855f3e80cdf85c231872b897f41f78624e38bd56da6a854462a3f8f35b4`  
		Last Modified: Wed, 10 Mar 2021 21:45:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2546886727759053cccfd44ac8d85642584457230bdba944f6651dff8ac8bca`  
		Last Modified: Wed, 10 Mar 2021 21:45:20 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2416a88d556dc24e1284df7253ea7257a39f1229564525254f095238f48fc97`  
		Last Modified: Wed, 10 Mar 2021 21:45:20 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ba1c7f3b3b979941d8c0847592ab35f1f82980625a38c804d801b3fa68d7e6`  
		Last Modified: Wed, 10 Mar 2021 21:45:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed032ff3bbe44776ff76827c8edd4ec2164d69d37f472b2127113338b478214f`  
		Last Modified: Wed, 10 Mar 2021 21:45:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783d7b3e5da6311f30234890e25925493d5b34fc2344886a83084492d83f4583`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20049d238f731868cb3d762df8034faf5bc27ba7024494295013a7bdc5782f`  
		Last Modified: Wed, 10 Mar 2021 21:45:18 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c87ab0a491513801045b830deb77e44c71c6eca44368182459f8bf9ccbf94c`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aef85cb3e822cd1c013f9d9cd34377b55595a562fccdeb5829cbe29762d1565`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 326.1 KB (326117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321fc9e27c48d69216d1c39ccb8e630b835829091e6fec4a070f81b154952691`  
		Last Modified: Wed, 10 Mar 2021 21:45:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:78fd3e7c57ab3ba12695d70a80262c61da00210106587256cf437f1a9f1e061c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829264967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea8287af00bc3215176603b53641bd1d0bc6a88a00fa2e91b7f469fb5d6a9b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:37:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:38:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:38:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:38:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:38:41 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:38:43 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:38:44 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:38:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:38:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:38:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:38:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:38:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:38:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:38:54 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:38:55 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:39:49 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:39:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068d235fdc3605555e5f5f986d759f521d9fc2671fc912abe8901595d45d60ab`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a8c13b430e11f8559e49a7516ea0a3df917cf370a512811b24aa6df83f5f0`  
		Last Modified: Wed, 10 Mar 2021 21:45:54 GMT  
		Size: 21.9 MB (21890337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9f0a0d089389068aacce76a6586d1f849ebaf9deb2c0844d2f97c5b1902c3c`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff1be978ab7b3c0c69146b26b6a288d85f12c47eee96ac71cf6a7151566078`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e262b01df5d3b0cf7f18456e428addd58277b7ec59681df285c56631bd530c1f`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeff2c1d9364727bbb7a1de68846e419d9f653f5319da7efbaa323658c26b48`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dad64a77e48bef36bd455f70d9ad06b83544f388bcd8235c25080d45ae8970`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0239d3fcf5f548af5b0c3e7117effa43baef43188cd5a77f063d85387b1d9df`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc76feb0f670cf8be35090ebebe3c4643fa107f237656ca352b95f635993fca`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dee0f2604aa4735cb4916b33c70ea425fa47fdcf149332ff05a43279861bda`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0d846b47ba13cb71b100d80357ad7dc9df41e5baf3f9d9521c42612e609d0b`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2470c6dc6014a45e42ff9f92c2727e721495efd2b9589a5ac5c6f0b22c36490a`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e53076fc5ab0c6120d49ae633dd65d6a0c5a0e0f0e8b708e9e135a12554f067`  
		Last Modified: Wed, 10 Mar 2021 21:45:41 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b9bf97f40f7208eb4539982865006e193756f28a3c7465053d45a8d04c40b4`  
		Last Modified: Wed, 10 Mar 2021 21:45:41 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293df8564c0989a8e85113cf1a8bfdb517a8f6490b5aa9c2e35960aea24bf363`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1870d93517098ab98b14710fa207f6b05ef1366f8bcea48882f0d3baa7abc4`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac094dadecb74c0eb1d8562e2974563f9e7bb5f5dc047f11ec504530cc1a9f14`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ba123c5815bf1a003074b6a7fd124d45546d9807c1e03832c898f388970ae1`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 256.9 KB (256897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6008b4f137610cb112001da1d9980c6fe7689bbdbe6aae8aaf981ed841244e3`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-alpine`

```console
$ docker pull caddy@sha256:b8bb929696b1ba5b4bfe5a97725fc80ddc3f6732c4ea72ec5a39a5b92c5b9366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.0-beta.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:292728877c3fc821295b18467bead2be953dd9b0f0d460eeeffd6b6ba357ab4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14763931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1116ab784c1c43b47dc886cedb417f7c56de689bb60adc895f4538d10da87cc9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:11:13 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:11:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:11:14 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Sat, 06 Mar 2021 08:11:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:11:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:11:18 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:11:18 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:11:18 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:11:18 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:11:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:11:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:11:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:11:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:11:20 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:11:20 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:11:21 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:11:21 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:11:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5621b554e24c44d7f631f7f0d4697255d447db5706e62161700d99a967e772c0`  
		Last Modified: Sat, 06 Mar 2021 08:12:20 GMT  
		Size: 300.4 KB (300402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b5cc7d40fe5b30ae3330852ebd414b71cec7693439fa8ea967cceb1d417ce`  
		Last Modified: Sat, 06 Mar 2021 08:12:20 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e541183feba6e676730c42880d65c075b0b7905af7dbfe0d55009667a9619145`  
		Last Modified: Sat, 06 Mar 2021 08:12:23 GMT  
		Size: 11.6 MB (11645890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f70013118953696dc59d068edba771a221bac2000df2f75cae9e2c989e1e09`  
		Last Modified: Sat, 06 Mar 2021 08:12:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:69ed026d4046988c7cfdb7d092d38b051af05f515c2c582640359a3b320a19fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13898470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5128877c7baed77cfb7dc037f11121a9aec61949f983428060720076eddc3e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:49:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:49:59 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:49:59 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:50:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:50:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:50:07 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:50:08 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:50:09 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:50:10 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:50:11 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:50:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:50:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:50:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:50:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:50:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:50:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:50:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:50:19 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:50:20 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:50:21 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:50:23 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:50:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435d76e6be3eef1e1ee27e127fafe5a99f442a92a7467b0866c4fb65ba4113b`  
		Last Modified: Wed, 24 Feb 2021 18:51:20 GMT  
		Size: 300.5 KB (300516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed97964c38308666a2f1211f6a5cfb26159b76e7d37a3eb8a4928989c8f862`  
		Last Modified: Wed, 24 Feb 2021 18:51:21 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e773a4b13e9da28035f76451153afcdec1f2497b19749b811b7877ce7135779c`  
		Last Modified: Wed, 24 Feb 2021 18:51:24 GMT  
		Size: 11.0 MB (10969934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94dd2f7265c37d9eadfc580dec6754dfa426f11cb141b8ddbc8c5b2dc5a7681`  
		Last Modified: Wed, 24 Feb 2021 18:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:504dc03b283ba138bea4b2d69113a4d751d8c276f07a6b704cc4866fe57e424b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13677502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce15e29dded4c237de13a06d5c8681e93e97b392f9474dcef8630fc3f2b3a8e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:58:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:58:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:58:08 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:58:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:58:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:58:15 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:58:16 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:58:16 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:58:17 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:58:19 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:58:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:58:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:58:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:58:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:58:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:58:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:58:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:58:25 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:58:26 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:58:27 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:58:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:58:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57f6854a8c929241451c6d527ac6efdee08455ee8c27aed146be03c5ad806a`  
		Last Modified: Wed, 24 Feb 2021 18:59:25 GMT  
		Size: 299.7 KB (299665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52063aab834f7e32087615a6698bd11bcc3ade3eb55687eac04d726ab9beeb04`  
		Last Modified: Wed, 24 Feb 2021 18:59:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fbdd64ea7052537bb15fdf9afa804352448372aeef61c0fcdc27a4fce971d7`  
		Last Modified: Wed, 24 Feb 2021 18:59:29 GMT  
		Size: 10.9 MB (10947961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515983999c4dfe73c741f123ff20ea42405a945d46673dd1bfe2695c464b32bf`  
		Last Modified: Wed, 24 Feb 2021 18:59:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5e6321e0c3df5fdb54f8771ed7ecd084831c7bb1dcf89ff3bba906bb6c10280a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13643152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44faf6dde77510e96fd734df5810f321b01a0630c7fc25b94bc2ddd6fc7b980`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:48:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:48:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:48:05 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:48:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:48:11 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:48:12 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:48:12 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:48:13 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:48:14 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:48:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:48:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:48:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:48:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:48:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:48:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:48:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:48:19 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:48:20 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:48:21 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:48:22 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:48:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677d00efd0cb981b2b1ec36a240fce8a89ec062c22e82f307dc6d2651ba6563`  
		Last Modified: Wed, 24 Feb 2021 18:49:19 GMT  
		Size: 300.6 KB (300624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1840450bb57f5fddd099628bb8f9fd57e0b070b11c7f6156e3206be7ce97dae`  
		Last Modified: Wed, 24 Feb 2021 18:49:19 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5716ac42e1610a59f8df7b7f4c4c2a62e28f4a325b0ce932624885fda5acc450`  
		Last Modified: Wed, 24 Feb 2021 18:49:22 GMT  
		Size: 10.6 MB (10624970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bf56fedcfd9886bf3d4adadd089babeb8ba22acec7bd4e7a56382595ef6aa9`  
		Last Modified: Wed, 24 Feb 2021 18:49:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1bf3b5016c63ee5734915f350b9e29553419eeaf5fe24c1ccbe2daac07606465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13387481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25b9219d7eaa3e483ca62e74df67b8b41b392979867c8588cbd9ddcee0e0771`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 19:53:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 19:54:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 19:54:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:54:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 19:54:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 19:54:30 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 19:54:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 19:54:38 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 19:54:44 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 19:54:53 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:55:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:55:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:55:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:55:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:55:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:55:26 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:55:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:55:36 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:55:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:55:44 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:55:51 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 19:55:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbd40a596b750ffbee0cd1cf44fbaee64a6e8aff893818fd8de97c75ab7d420`  
		Last Modified: Wed, 24 Feb 2021 19:58:09 GMT  
		Size: 302.5 KB (302524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829bd2a32cf8c0482e15697e74af7944b770aa08730dfb0a976ac07db2290d6a`  
		Last Modified: Wed, 24 Feb 2021 19:58:09 GMT  
		Size: 5.8 KB (5837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74c34fc68a5ade6104fdc66c39bc89fa91b5169d51d4ad8e6c5c793bfa450db`  
		Last Modified: Wed, 24 Feb 2021 19:58:11 GMT  
		Size: 10.3 MB (10265885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dee8547b806efa1a0876f5c3fcb41f5f5e5374df0602acc3a31d49892bbeb3`  
		Last Modified: Wed, 24 Feb 2021 19:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0c9cd2a968cf969ece10e66e605defb77deb94024fa4c713e6ad63cfd7ec8762
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14199778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fcb091c13bf8102a1e374393ddeebc38c4096b89dbaed3a48c3aa723f7f336f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 20:41:27 GMT
ADD file:630c66f8d774d75b51e32aff812b438d377ebd3389c4aa6c324fdf8c03b6fa13 in / 
# Wed, 17 Feb 2021 20:41:27 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 18:41:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 18:41:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 18:41:51 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 18:41:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 18:42:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 18:42:00 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 18:42:00 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 18:42:01 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:42:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 18:42:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 18:42:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 18:42:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 18:42:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 18:42:06 GMT
EXPOSE 80
# Wed, 24 Feb 2021 18:42:07 GMT
EXPOSE 443
# Wed, 24 Feb 2021 18:42:07 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 18:42:08 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 18:42:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ff5e8cb87555e9fa38a441f5cf0414e91353e2cd21cdb48d48b7de5bb39ce674`  
		Last Modified: Wed, 17 Feb 2021 20:41:58 GMT  
		Size: 2.6 MB (2602381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3fdfa6c58844c6cc4a07b66ee1ef0a17f8699df726982b254ff58a2117abd1`  
		Last Modified: Wed, 24 Feb 2021 18:42:52 GMT  
		Size: 300.8 KB (300837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bdb77fb831f3e597bfccda2296099260d12b7e671c7697a6f722c1af54f650`  
		Last Modified: Wed, 24 Feb 2021 18:42:53 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c299797220d87efdd996a17402dcd1e747734ac17c3f524fcdb8d5a0b4f4cccd`  
		Last Modified: Wed, 24 Feb 2021 18:42:59 GMT  
		Size: 11.3 MB (11290578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1c503c26851e352a5fe95cb24e8a73b2a5d10539ea54d80325f801441190de`  
		Last Modified: Wed, 24 Feb 2021 18:42:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder`

```console
$ docker pull caddy@sha256:15798f387dbb7723ff4e3598a6d6a67b1e3965f414042c87bb3dfbc7540d5b11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:5823657a11ee58244ae63737da85c16fc639a39025eb3b1bc3a4c7c862eff5d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116486038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c50b7fa80eecafffe6e7f52fd89da6afbecb8002a98f28e533aad0174e1f19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:35:03 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:35:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:35:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:20:28 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:22:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:22:11 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:22:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:22:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:22:12 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:28 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:28 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 22:49:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:30 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448433d692de67fadc3e270369294f10bbc32683e28e4144e7d2d2fedbf60756`  
		Last Modified: Sat, 06 Mar 2021 01:45:56 GMT  
		Size: 281.3 KB (281267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a3d42746fcfc7f036d78c91f23a708eccc332efd705161238e6aafc5535a9`  
		Last Modified: Sat, 06 Mar 2021 01:45:55 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d283d788a6f5f59325116bda7d61102a1bc7f74d902d617ed62cf90c58fdc6`  
		Last Modified: Thu, 11 Mar 2021 22:30:50 GMT  
		Size: 105.7 MB (105693502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757f90a0dc844e1ca0ce652556adf5fddaaab3b13d949b52fc384525af8c894e`  
		Last Modified: Thu, 11 Mar 2021 22:30:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0bfdc443a1ef0ce6cb86012da84b6245f2f00a2862f4e9f6984fa76942f7e6`  
		Last Modified: Thu, 11 Mar 2021 22:50:18 GMT  
		Size: 6.4 MB (6387824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459bf636a007ea65edfb16a1c95e14148a8c64f9be6ea5ff26185b7aae7bde6a`  
		Last Modified: Thu, 11 Mar 2021 22:50:13 GMT  
		Size: 1.3 MB (1311073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef54d0358b38ccc7b14b30689f1dc074db2901ae54d07d3a04d8b0a9356ded`  
		Last Modified: Thu, 11 Mar 2021 22:50:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:8f7483f8feb4e1782c34ffa997cd5efd02a8366d6d858b1514988c53a5d471d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112245143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef1ac5c77087a72d6f4ab2696fb11c3a1dd4062ef5870f1cd5adaae64c35497`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:13:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:13:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:13:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:48 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:54:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:54:57 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:54:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:55:01 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:25:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:25:06 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:25:07 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:25:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:25:11 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:25:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1115ea1bf3d04fcf67e0e6cae415e63d7f357abb70d3f7856dd5aa03de896ecc`  
		Last Modified: Wed, 17 Feb 2021 21:21:04 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c994967e2e16efef7e77241efa59bfd4a5b5c60495cd92dbc5b17c1d8ddd8c00`  
		Last Modified: Wed, 17 Feb 2021 21:21:03 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0689fa2d4b19ee5c634094c69a00240654bee99966bb3a37093e234f6cf20224`  
		Last Modified: Thu, 11 Mar 2021 23:06:46 GMT  
		Size: 101.9 MB (101894352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2fb2bdc628634dd6d49677e992f2124f671184553719a258308f7997bb4c00`  
		Last Modified: Thu, 11 Mar 2021 23:06:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19589d7ff76255f1ade4021f598f6eae157f9fef852f3104ffd4fac4d5b3ed49`  
		Last Modified: Thu, 11 Mar 2021 23:25:49 GMT  
		Size: 6.2 MB (6225075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d38eb1a39e7fd0460387f47331e8e8a618b4fae1ec802b552946767816b550`  
		Last Modified: Thu, 11 Mar 2021 23:25:47 GMT  
		Size: 1.2 MB (1221591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37d8db5d71ab993bfa66effcf9fbd023b87cdef0e201dd88dc5fdbc3f083ea9`  
		Last Modified: Thu, 11 Mar 2021 23:25:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:18bb4d8d3017276b58c655d844b55f9c4fd2a98b86dd7eda202e3b925fb18fb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111178931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76743156a1dbfbc03522f064146553f87f7dc11fc5047e73f485c89e3e949b6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:40:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:40:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:40:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:01:12 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 23:03:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:03:54 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:03:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:03:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:03:58 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:36 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:37 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:58:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcbf0a74807f56302ee496bfb362a280b21aa9c4fdeecc46895ac701f5bca1c`  
		Last Modified: Wed, 17 Feb 2021 21:46:54 GMT  
		Size: 280.5 KB (280527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c30d8b16ab97329386be2d5f27303fe56597db77aa98347479208746583bf82`  
		Last Modified: Wed, 17 Feb 2021 21:46:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567159374ba5633dbaee16d927c5e616da634bf3e4bde5fe4b9b91c069ad3fd`  
		Last Modified: Thu, 11 Mar 2021 23:16:30 GMT  
		Size: 101.7 MB (101696170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40abf8cd21c4c461b4dd2fd8065151528b7bced925aa04ac9672368012510386`  
		Last Modified: Thu, 11 Mar 2021 23:16:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fc60d512ea1bc22b41c016814915d944ad67b66f438ef60e7cb50d39d6abd6`  
		Last Modified: Thu, 11 Mar 2021 23:59:25 GMT  
		Size: 5.6 MB (5558178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21208a7f50c0664676ee537f2513a992bf9290d8a38426b71e4c10f27169b081`  
		Last Modified: Thu, 11 Mar 2021 23:59:23 GMT  
		Size: 1.2 MB (1219449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8391c4ca16dd4dceb4df49e4d1dd8d5166894e9380883cce2c7c08983db14e7`  
		Last Modified: Thu, 11 Mar 2021 23:59:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9859951106eaaa99c5b81a2b41a3010d8a179684fc3713fa124eb360a3d720a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111679768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520e384613881c176aa28d672d0a2b689d510a1cd6ab78abb09e0f2c908742dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:28:29 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:28:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:28:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:40:56 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:43:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:43:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:43:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:43:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:43:28 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:39 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:13:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c12b87152786d4aecdcab19bf08c376457c5a28279d38b48a67be496f0ffac`  
		Last Modified: Wed, 17 Feb 2021 21:34:04 GMT  
		Size: 281.5 KB (281481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e198097068c506d482e6e3a24c9e93ad44c60822816f52bc743d767fd2bbc`  
		Last Modified: Wed, 17 Feb 2021 21:34:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6948a1906ae692419137d9db26a066c5d9e4fd87dcc03dd0727d1f009d80832`  
		Last Modified: Thu, 11 Mar 2021 22:54:03 GMT  
		Size: 101.0 MB (101010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85154f35e78178bdc5002c4be44c626d49b441090037be5b88961f1a89a05f15`  
		Last Modified: Thu, 11 Mar 2021 22:53:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e5c3c3f2bb89c7b1c7783da101056f60e83d0fc51f76777ae42c110c0805cf`  
		Last Modified: Thu, 11 Mar 2021 23:14:29 GMT  
		Size: 6.5 MB (6474034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13501cae18cc7558a3f93f7bdff324526a01fb89e13a3d88489ab82b4e2b23ba`  
		Last Modified: Thu, 11 Mar 2021 23:14:28 GMT  
		Size: 1.2 MB (1201554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f14ee36743e248669e492b767507d3e495928cd209b20ba4065cdd80417de`  
		Last Modified: Thu, 11 Mar 2021 23:14:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:fb18b1fc02172faedc71d4218355d44f1f9293be055750c5d6ea69ec5a7d7a42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110575542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75edba5e6dd624b6b0e5d3807f77619b5d9b6f5222b41ac6a880f61aaa66e971`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:00:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 22:00:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 22:01:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:10:19 GMT
ENV GOLANG_VERSION=1.16.2
# Fri, 12 Mar 2021 00:12:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:13:04 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:13:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:13:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:13:49 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:52:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:53:02 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:53:11 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 12 Mar 2021 00:53:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:53:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:53:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b4ebc7d414e7ac070e49eb931df4dd465ce13296bd4c84782943833dbc6424`  
		Last Modified: Wed, 17 Feb 2021 22:08:30 GMT  
		Size: 283.4 KB (283402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8666f55b6dcdfcc51dc8bda03a868809a3bf882d5f753f4b717e558256912157`  
		Last Modified: Wed, 17 Feb 2021 22:08:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6fc0e5bf71c82f266733c62f2cfd9a02fd12fd4e7918c5eb1738280a3c8f0`  
		Last Modified: Fri, 12 Mar 2021 00:30:52 GMT  
		Size: 99.5 MB (99484635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725d6003452d597ac8ea574377577ccca7eb1014a93bfedebb0720e442fa0340`  
		Last Modified: Fri, 12 Mar 2021 00:28:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c87a64a4fb57313aaac6260dfecd4ea5cbe0e99678c0c4d62998586b7db0e7`  
		Last Modified: Fri, 12 Mar 2021 00:54:21 GMT  
		Size: 6.8 MB (6823216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a878ae1859958775375d8ac5bc770d2d064154b3e4da16a6d6359a90485b0c0d`  
		Last Modified: Fri, 12 Mar 2021 00:54:20 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b803ed7a9a362acd1778815eac92039ea009b7675a5588d47a74e9203ae57309`  
		Last Modified: Fri, 12 Mar 2021 00:54:20 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:f7c0d3918d6384e0dd736122e0806f4b7480e976ea41bb075722b13409bb98c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115411796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e49eda5b3c3cbfdf4f87849d69dd13dd2f97eae886904b49d96c18f2442ef26`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:41:27 GMT
ADD file:630c66f8d774d75b51e32aff812b438d377ebd3389c4aa6c324fdf8c03b6fa13 in / 
# Wed, 17 Feb 2021 20:41:27 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:16 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:24:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:24:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:42:37 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:45:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:45:54 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:45:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:45:57 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:14:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:14:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:14:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:14:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:14:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:14:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:14:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ff5e8cb87555e9fa38a441f5cf0414e91353e2cd21cdb48d48b7de5bb39ce674`  
		Last Modified: Wed, 17 Feb 2021 20:41:58 GMT  
		Size: 2.6 MB (2602381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd069c36ed60b5dee3feb6db7c60b266e42ee2b431eba05eeb7e347fd68900d`  
		Last Modified: Wed, 17 Feb 2021 21:32:05 GMT  
		Size: 281.7 KB (281699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861c0a8bd2a308974e4214b26d53277219346795ffc47e9badca7625c1532799`  
		Last Modified: Wed, 17 Feb 2021 21:32:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b40c2f406f64eb8ef939b1143b5317d7b58c5524c2387047f5b97090441086b`  
		Last Modified: Thu, 11 Mar 2021 22:56:30 GMT  
		Size: 104.8 MB (104790688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550af5ec596d126d1269d1c89f457104a8a73fc777ef6fef2ece5ea9ab33f339`  
		Last Modified: Thu, 11 Mar 2021 22:56:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948d54fc4d27a449d5ee8bc6ced2ff778a14c8af94ef147b1ad1da988b992117`  
		Last Modified: Thu, 11 Mar 2021 23:14:46 GMT  
		Size: 6.5 MB (6471889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c45d0b461ea7ec5a7f3ca3269dc0e27b2276314e393a83f70dad1d78119d8e8`  
		Last Modified: Thu, 11 Mar 2021 23:14:45 GMT  
		Size: 1.3 MB (1264424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8029a7baaa337e887b003fa890c8cbd7e694462738c7c5ddf030fedb96b27be5`  
		Last Modified: Thu, 11 Mar 2021 23:14:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:e104a1833b67510fa0a05f4f924a67a864d2e5e9df48e474fe694c8c448d7a3d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2641915003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f733f062c7d3dc2aa52a2921fb022e89181346b705d2d5a2361ab724083069f3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:15:26 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 23:18:15 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'baa7d69482365930ecc5c0b99e6a5935180988a2e7b49aa8a22dbcd39f4064b7'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:18:17 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:06:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:06:41 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:06:42 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 12 Mar 2021 00:06:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:07:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:07:12 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9537bc155f15b30642aa7b63f0679ed8d5f083b5d5fa037c40c41135bd39b8f7`  
		Last Modified: Thu, 11 Mar 2021 23:37:17 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146bc0a51ffa75749c1d8bb1d46c6becf001283c33e85bb2240220338876e95d`  
		Last Modified: Thu, 11 Mar 2021 23:40:09 GMT  
		Size: 143.8 MB (143753308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf3db5037d83a1a71a6947d32e46ee6c0976e079b1ae65a13e8bcaecf1508b3`  
		Last Modified: Thu, 11 Mar 2021 23:37:17 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94f7b005001b282c649a02bb53cd5903aaea5da5a13157c30479852ac46e19d`  
		Last Modified: Fri, 12 Mar 2021 00:10:49 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6223e5bbc83fc2c069bf773bc4b9437fe5f5280d92e58500aabb6913405c6db`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03eb709eb889f22d23ab0cfe46094174915807a8606b073105dd447d87e5b53`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15cafbc373b7fd4a53829fb85ce882c8905275fcdd54a10228ee5dd397039cc`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ce8ebc80f5a559b20fd3b0a903effa8cc9a05fa7bbe6728fb7bdcee65bdf84`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.7 MB (1729691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb1a4fa274df46b7e8270f4d82a030cfdad4d047d56b0280bc7adf2b03d79d5`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:777513a65701c4ae3ce5904c4c1967b28241df6fdb53b137a41bb751fc55dcc3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6003031122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4176570aedb88fcb75cf8dd882ea028fb6975b8ffdc3992209c284aac50c218`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:18:39 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 23:22:37 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'baa7d69482365930ecc5c0b99e6a5935180988a2e7b49aa8a22dbcd39f4064b7'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:22:39 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:07:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:07:19 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:07:20 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 12 Mar 2021 00:07:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:08:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:08:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bf119dffbcda81258f3b57891db300e915d66e2fac3f436c4bd3d3df153d7`  
		Last Modified: Thu, 11 Mar 2021 23:40:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fea2922e7872b2f55d2c7458491386a7ae934cda27a555e1d7fd2e2d7caf59`  
		Last Modified: Thu, 11 Mar 2021 23:41:04 GMT  
		Size: 149.2 MB (149168243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb93cea29b321ba452f4f7fcb2714e52d422275f4e04918dfebf877182d2df10`  
		Last Modified: Thu, 11 Mar 2021 23:40:30 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645dc3727c20265e28a3de6d031c38028ad7f48f361685317c4a1873feea106f`  
		Last Modified: Fri, 12 Mar 2021 00:10:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a936392e185bbdc39c57fa14491962bbd59f1a54d7db6c7c74ccfbc63d2ccee5`  
		Last Modified: Fri, 12 Mar 2021 00:11:00 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbca6efdfdc926c0911d1b618c998506fc19962acd11543beae442b11897b7a`  
		Last Modified: Fri, 12 Mar 2021 00:10:57 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ab77ddd91507ec680c4e923ef3e0ee3ab41971cc582bdd9899d957cbc4581`  
		Last Modified: Fri, 12 Mar 2021 00:10:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb40c7e366cf59923f8d7e014a15a7b671314c0b46056de677ca6c37bcd0c2d`  
		Last Modified: Fri, 12 Mar 2021 00:11:11 GMT  
		Size: 11.5 MB (11521093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a578909e723402a1acc91db9a593ed2c998cda230ae74476c53ff325178cc10d`  
		Last Modified: Fri, 12 Mar 2021 00:10:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder-alpine`

```console
$ docker pull caddy@sha256:000e35bc1fcd519c3e4da25f76f8a14d0bc0ee1730e25816c984e7fbd4f3d910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.0-beta.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:5823657a11ee58244ae63737da85c16fc639a39025eb3b1bc3a4c7c862eff5d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116486038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c50b7fa80eecafffe6e7f52fd89da6afbecb8002a98f28e533aad0174e1f19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:35:03 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:35:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:35:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:20:28 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:22:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:22:11 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:22:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:22:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:22:12 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:28 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:28 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 22:49:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:30 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448433d692de67fadc3e270369294f10bbc32683e28e4144e7d2d2fedbf60756`  
		Last Modified: Sat, 06 Mar 2021 01:45:56 GMT  
		Size: 281.3 KB (281267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a3d42746fcfc7f036d78c91f23a708eccc332efd705161238e6aafc5535a9`  
		Last Modified: Sat, 06 Mar 2021 01:45:55 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d283d788a6f5f59325116bda7d61102a1bc7f74d902d617ed62cf90c58fdc6`  
		Last Modified: Thu, 11 Mar 2021 22:30:50 GMT  
		Size: 105.7 MB (105693502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757f90a0dc844e1ca0ce652556adf5fddaaab3b13d949b52fc384525af8c894e`  
		Last Modified: Thu, 11 Mar 2021 22:30:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0bfdc443a1ef0ce6cb86012da84b6245f2f00a2862f4e9f6984fa76942f7e6`  
		Last Modified: Thu, 11 Mar 2021 22:50:18 GMT  
		Size: 6.4 MB (6387824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459bf636a007ea65edfb16a1c95e14148a8c64f9be6ea5ff26185b7aae7bde6a`  
		Last Modified: Thu, 11 Mar 2021 22:50:13 GMT  
		Size: 1.3 MB (1311073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef54d0358b38ccc7b14b30689f1dc074db2901ae54d07d3a04d8b0a9356ded`  
		Last Modified: Thu, 11 Mar 2021 22:50:13 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:8f7483f8feb4e1782c34ffa997cd5efd02a8366d6d858b1514988c53a5d471d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112245143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef1ac5c77087a72d6f4ab2696fb11c3a1dd4062ef5870f1cd5adaae64c35497`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:13:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:13:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:13:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:48 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:54:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:54:57 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:54:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:55:01 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:25:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:25:06 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:25:07 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:25:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:25:11 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:25:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1115ea1bf3d04fcf67e0e6cae415e63d7f357abb70d3f7856dd5aa03de896ecc`  
		Last Modified: Wed, 17 Feb 2021 21:21:04 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c994967e2e16efef7e77241efa59bfd4a5b5c60495cd92dbc5b17c1d8ddd8c00`  
		Last Modified: Wed, 17 Feb 2021 21:21:03 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0689fa2d4b19ee5c634094c69a00240654bee99966bb3a37093e234f6cf20224`  
		Last Modified: Thu, 11 Mar 2021 23:06:46 GMT  
		Size: 101.9 MB (101894352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2fb2bdc628634dd6d49677e992f2124f671184553719a258308f7997bb4c00`  
		Last Modified: Thu, 11 Mar 2021 23:06:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19589d7ff76255f1ade4021f598f6eae157f9fef852f3104ffd4fac4d5b3ed49`  
		Last Modified: Thu, 11 Mar 2021 23:25:49 GMT  
		Size: 6.2 MB (6225075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d38eb1a39e7fd0460387f47331e8e8a618b4fae1ec802b552946767816b550`  
		Last Modified: Thu, 11 Mar 2021 23:25:47 GMT  
		Size: 1.2 MB (1221591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37d8db5d71ab993bfa66effcf9fbd023b87cdef0e201dd88dc5fdbc3f083ea9`  
		Last Modified: Thu, 11 Mar 2021 23:25:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:18bb4d8d3017276b58c655d844b55f9c4fd2a98b86dd7eda202e3b925fb18fb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111178931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76743156a1dbfbc03522f064146553f87f7dc11fc5047e73f485c89e3e949b6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:40:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:40:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:40:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:01:12 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 23:03:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:03:54 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:03:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:03:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:03:58 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:36 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:37 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:58:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcbf0a74807f56302ee496bfb362a280b21aa9c4fdeecc46895ac701f5bca1c`  
		Last Modified: Wed, 17 Feb 2021 21:46:54 GMT  
		Size: 280.5 KB (280527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c30d8b16ab97329386be2d5f27303fe56597db77aa98347479208746583bf82`  
		Last Modified: Wed, 17 Feb 2021 21:46:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567159374ba5633dbaee16d927c5e616da634bf3e4bde5fe4b9b91c069ad3fd`  
		Last Modified: Thu, 11 Mar 2021 23:16:30 GMT  
		Size: 101.7 MB (101696170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40abf8cd21c4c461b4dd2fd8065151528b7bced925aa04ac9672368012510386`  
		Last Modified: Thu, 11 Mar 2021 23:16:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fc60d512ea1bc22b41c016814915d944ad67b66f438ef60e7cb50d39d6abd6`  
		Last Modified: Thu, 11 Mar 2021 23:59:25 GMT  
		Size: 5.6 MB (5558178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21208a7f50c0664676ee537f2513a992bf9290d8a38426b71e4c10f27169b081`  
		Last Modified: Thu, 11 Mar 2021 23:59:23 GMT  
		Size: 1.2 MB (1219449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8391c4ca16dd4dceb4df49e4d1dd8d5166894e9380883cce2c7c08983db14e7`  
		Last Modified: Thu, 11 Mar 2021 23:59:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9859951106eaaa99c5b81a2b41a3010d8a179684fc3713fa124eb360a3d720a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111679768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520e384613881c176aa28d672d0a2b689d510a1cd6ab78abb09e0f2c908742dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:28:29 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:28:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:28:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:40:56 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:43:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:43:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:43:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:43:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:43:28 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:39 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:13:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c12b87152786d4aecdcab19bf08c376457c5a28279d38b48a67be496f0ffac`  
		Last Modified: Wed, 17 Feb 2021 21:34:04 GMT  
		Size: 281.5 KB (281481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657e198097068c506d482e6e3a24c9e93ad44c60822816f52bc743d767fd2bbc`  
		Last Modified: Wed, 17 Feb 2021 21:34:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6948a1906ae692419137d9db26a066c5d9e4fd87dcc03dd0727d1f009d80832`  
		Last Modified: Thu, 11 Mar 2021 22:54:03 GMT  
		Size: 101.0 MB (101010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85154f35e78178bdc5002c4be44c626d49b441090037be5b88961f1a89a05f15`  
		Last Modified: Thu, 11 Mar 2021 22:53:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e5c3c3f2bb89c7b1c7783da101056f60e83d0fc51f76777ae42c110c0805cf`  
		Last Modified: Thu, 11 Mar 2021 23:14:29 GMT  
		Size: 6.5 MB (6474034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13501cae18cc7558a3f93f7bdff324526a01fb89e13a3d88489ab82b4e2b23ba`  
		Last Modified: Thu, 11 Mar 2021 23:14:28 GMT  
		Size: 1.2 MB (1201554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f14ee36743e248669e492b767507d3e495928cd209b20ba4065cdd80417de`  
		Last Modified: Thu, 11 Mar 2021 23:14:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:fb18b1fc02172faedc71d4218355d44f1f9293be055750c5d6ea69ec5a7d7a42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110575542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75edba5e6dd624b6b0e5d3807f77619b5d9b6f5222b41ac6a880f61aaa66e971`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:00:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 22:00:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 22:01:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:10:19 GMT
ENV GOLANG_VERSION=1.16.2
# Fri, 12 Mar 2021 00:12:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:13:04 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:13:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:13:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:13:49 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:52:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:53:02 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:53:11 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 12 Mar 2021 00:53:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:53:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:53:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:53:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b4ebc7d414e7ac070e49eb931df4dd465ce13296bd4c84782943833dbc6424`  
		Last Modified: Wed, 17 Feb 2021 22:08:30 GMT  
		Size: 283.4 KB (283402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8666f55b6dcdfcc51dc8bda03a868809a3bf882d5f753f4b717e558256912157`  
		Last Modified: Wed, 17 Feb 2021 22:08:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6fc0e5bf71c82f266733c62f2cfd9a02fd12fd4e7918c5eb1738280a3c8f0`  
		Last Modified: Fri, 12 Mar 2021 00:30:52 GMT  
		Size: 99.5 MB (99484635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725d6003452d597ac8ea574377577ccca7eb1014a93bfedebb0720e442fa0340`  
		Last Modified: Fri, 12 Mar 2021 00:28:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c87a64a4fb57313aaac6260dfecd4ea5cbe0e99678c0c4d62998586b7db0e7`  
		Last Modified: Fri, 12 Mar 2021 00:54:21 GMT  
		Size: 6.8 MB (6823216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a878ae1859958775375d8ac5bc770d2d064154b3e4da16a6d6359a90485b0c0d`  
		Last Modified: Fri, 12 Mar 2021 00:54:20 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b803ed7a9a362acd1778815eac92039ea009b7675a5588d47a74e9203ae57309`  
		Last Modified: Fri, 12 Mar 2021 00:54:20 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f7c0d3918d6384e0dd736122e0806f4b7480e976ea41bb075722b13409bb98c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115411796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e49eda5b3c3cbfdf4f87849d69dd13dd2f97eae886904b49d96c18f2442ef26`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 20:41:27 GMT
ADD file:630c66f8d774d75b51e32aff812b438d377ebd3389c4aa6c324fdf8c03b6fa13 in / 
# Wed, 17 Feb 2021 20:41:27 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:16 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 21:24:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 21:24:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:42:37 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 22:45:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:45:54 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:45:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:45:57 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:14:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:14:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:14:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 11 Mar 2021 23:14:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:14:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:14:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:14:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ff5e8cb87555e9fa38a441f5cf0414e91353e2cd21cdb48d48b7de5bb39ce674`  
		Last Modified: Wed, 17 Feb 2021 20:41:58 GMT  
		Size: 2.6 MB (2602381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd069c36ed60b5dee3feb6db7c60b266e42ee2b431eba05eeb7e347fd68900d`  
		Last Modified: Wed, 17 Feb 2021 21:32:05 GMT  
		Size: 281.7 KB (281699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861c0a8bd2a308974e4214b26d53277219346795ffc47e9badca7625c1532799`  
		Last Modified: Wed, 17 Feb 2021 21:32:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b40c2f406f64eb8ef939b1143b5317d7b58c5524c2387047f5b97090441086b`  
		Last Modified: Thu, 11 Mar 2021 22:56:30 GMT  
		Size: 104.8 MB (104790688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550af5ec596d126d1269d1c89f457104a8a73fc777ef6fef2ece5ea9ab33f339`  
		Last Modified: Thu, 11 Mar 2021 22:56:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948d54fc4d27a449d5ee8bc6ced2ff778a14c8af94ef147b1ad1da988b992117`  
		Last Modified: Thu, 11 Mar 2021 23:14:46 GMT  
		Size: 6.5 MB (6471889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c45d0b461ea7ec5a7f3ca3269dc0e27b2276314e393a83f70dad1d78119d8e8`  
		Last Modified: Thu, 11 Mar 2021 23:14:45 GMT  
		Size: 1.3 MB (1264424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8029a7baaa337e887b003fa890c8cbd7e694462738c7c5ddf030fedb96b27be5`  
		Last Modified: Thu, 11 Mar 2021 23:14:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a9a3bdf486699a1d7fa037327fbe650d3acce2d54d8bf5d1e5282f1d1d3a6fdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.4.0-beta.1-builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:e104a1833b67510fa0a05f4f924a67a864d2e5e9df48e474fe694c8c448d7a3d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2641915003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f733f062c7d3dc2aa52a2921fb022e89181346b705d2d5a2361ab724083069f3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:15:26 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 23:18:15 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'baa7d69482365930ecc5c0b99e6a5935180988a2e7b49aa8a22dbcd39f4064b7'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:18:17 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:06:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:06:41 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:06:42 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 12 Mar 2021 00:06:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:07:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:07:12 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9537bc155f15b30642aa7b63f0679ed8d5f083b5d5fa037c40c41135bd39b8f7`  
		Last Modified: Thu, 11 Mar 2021 23:37:17 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146bc0a51ffa75749c1d8bb1d46c6becf001283c33e85bb2240220338876e95d`  
		Last Modified: Thu, 11 Mar 2021 23:40:09 GMT  
		Size: 143.8 MB (143753308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf3db5037d83a1a71a6947d32e46ee6c0976e079b1ae65a13e8bcaecf1508b3`  
		Last Modified: Thu, 11 Mar 2021 23:37:17 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94f7b005001b282c649a02bb53cd5903aaea5da5a13157c30479852ac46e19d`  
		Last Modified: Fri, 12 Mar 2021 00:10:49 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6223e5bbc83fc2c069bf773bc4b9437fe5f5280d92e58500aabb6913405c6db`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03eb709eb889f22d23ab0cfe46094174915807a8606b073105dd447d87e5b53`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15cafbc373b7fd4a53829fb85ce882c8905275fcdd54a10228ee5dd397039cc`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ce8ebc80f5a559b20fd3b0a903effa8cc9a05fa7bbe6728fb7bdcee65bdf84`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.7 MB (1729691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb1a4fa274df46b7e8270f4d82a030cfdad4d047d56b0280bc7adf2b03d79d5`  
		Last Modified: Fri, 12 Mar 2021 00:10:46 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:3d8bb0ce374f35fbfc52f7aa44132199ce85323e8f9a6942b7a3a575afebbb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:777513a65701c4ae3ce5904c4c1967b28241df6fdb53b137a41bb751fc55dcc3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6003031122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4176570aedb88fcb75cf8dd882ea028fb6975b8ffdc3992209c284aac50c218`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:18:39 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 11 Mar 2021 23:22:37 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'baa7d69482365930ecc5c0b99e6a5935180988a2e7b49aa8a22dbcd39f4064b7'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:22:39 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:07:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:07:19 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:07:20 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 12 Mar 2021 00:07:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:08:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:08:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bf119dffbcda81258f3b57891db300e915d66e2fac3f436c4bd3d3df153d7`  
		Last Modified: Thu, 11 Mar 2021 23:40:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fea2922e7872b2f55d2c7458491386a7ae934cda27a555e1d7fd2e2d7caf59`  
		Last Modified: Thu, 11 Mar 2021 23:41:04 GMT  
		Size: 149.2 MB (149168243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb93cea29b321ba452f4f7fcb2714e52d422275f4e04918dfebf877182d2df10`  
		Last Modified: Thu, 11 Mar 2021 23:40:30 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645dc3727c20265e28a3de6d031c38028ad7f48f361685317c4a1873feea106f`  
		Last Modified: Fri, 12 Mar 2021 00:10:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a936392e185bbdc39c57fa14491962bbd59f1a54d7db6c7c74ccfbc63d2ccee5`  
		Last Modified: Fri, 12 Mar 2021 00:11:00 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbca6efdfdc926c0911d1b618c998506fc19962acd11543beae442b11897b7a`  
		Last Modified: Fri, 12 Mar 2021 00:10:57 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ab77ddd91507ec680c4e923ef3e0ee3ab41971cc582bdd9899d957cbc4581`  
		Last Modified: Fri, 12 Mar 2021 00:10:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb40c7e366cf59923f8d7e014a15a7b671314c0b46056de677ca6c37bcd0c2d`  
		Last Modified: Fri, 12 Mar 2021 00:11:11 GMT  
		Size: 11.5 MB (11521093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a578909e723402a1acc91db9a593ed2c998cda230ae74476c53ff325178cc10d`  
		Last Modified: Fri, 12 Mar 2021 00:10:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-windowsservercore`

```console
$ docker pull caddy@sha256:7108cf969c25357cbd77c97d7dd54879e4eecbbb597e66fd04517e084e9be88c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.1-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:6e5d5fea5cb01c12f4a392581b1d7cd9c8d057edf35421f107831ac987426788
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487833197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d9298e9342ee167543a1f5ea16eb3acde3c3e78c807d7d27b76ed6bc7587f9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:35:55 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:36:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:36:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:36:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:36:29 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:36:31 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:36:32 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:36:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:36:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:36:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:36:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:36:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:36:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:36:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:36:40 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:36:41 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:36:42 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:37:01 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:37:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc803029bd3ef109ba5043ff19061940f4d933b3b12efaadce4d958fff6984b`  
		Last Modified: Wed, 10 Mar 2021 21:45:26 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e23f022464526cb08cf5ae2524d4194aeb092d552b2a12309a02e731b92f2d`  
		Last Modified: Wed, 10 Mar 2021 21:45:30 GMT  
		Size: 16.5 MB (16480793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4417b70d9203a0f38da3e90189d96fca91c20a89c9f840dc3bf64b4f2561ae5c`  
		Last Modified: Wed, 10 Mar 2021 21:45:26 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4755067618a3cdc748f363c5f1a3da8eef0324233e5927f7dbac370b44bdc0`  
		Last Modified: Wed, 10 Mar 2021 21:45:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a4666bc7b476eb9b14bea25d19716eabf278bcba06df2e012e67a38477aa6`  
		Last Modified: Wed, 10 Mar 2021 21:45:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1c2bc1c49e7b0cba9e9ca161fc75374d674e2149ea25c38cf3ceeb9ce2cd5c`  
		Last Modified: Wed, 10 Mar 2021 21:45:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8c6b745994cb1e2bf9dcd0d2819313119ebc53c3fe9b49cdae27bad55cd4ab`  
		Last Modified: Wed, 10 Mar 2021 21:45:23 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0539021a8993cee20a823ee8225ec8615125fa5e331639602e11912f8a3e03c2`  
		Last Modified: Wed, 10 Mar 2021 21:45:24 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dbc014cc64499a05b9a2c7672e407fcf64a2c92e931fb4459f0a576d56d5fd`  
		Last Modified: Wed, 10 Mar 2021 21:45:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1bd855f3e80cdf85c231872b897f41f78624e38bd56da6a854462a3f8f35b4`  
		Last Modified: Wed, 10 Mar 2021 21:45:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2546886727759053cccfd44ac8d85642584457230bdba944f6651dff8ac8bca`  
		Last Modified: Wed, 10 Mar 2021 21:45:20 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2416a88d556dc24e1284df7253ea7257a39f1229564525254f095238f48fc97`  
		Last Modified: Wed, 10 Mar 2021 21:45:20 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ba1c7f3b3b979941d8c0847592ab35f1f82980625a38c804d801b3fa68d7e6`  
		Last Modified: Wed, 10 Mar 2021 21:45:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed032ff3bbe44776ff76827c8edd4ec2164d69d37f472b2127113338b478214f`  
		Last Modified: Wed, 10 Mar 2021 21:45:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783d7b3e5da6311f30234890e25925493d5b34fc2344886a83084492d83f4583`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20049d238f731868cb3d762df8034faf5bc27ba7024494295013a7bdc5782f`  
		Last Modified: Wed, 10 Mar 2021 21:45:18 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c87ab0a491513801045b830deb77e44c71c6eca44368182459f8bf9ccbf94c`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aef85cb3e822cd1c013f9d9cd34377b55595a562fccdeb5829cbe29762d1565`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 326.1 KB (326117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321fc9e27c48d69216d1c39ccb8e630b835829091e6fec4a070f81b154952691`  
		Last Modified: Wed, 10 Mar 2021 21:45:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:78fd3e7c57ab3ba12695d70a80262c61da00210106587256cf437f1a9f1e061c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829264967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea8287af00bc3215176603b53641bd1d0bc6a88a00fa2e91b7f469fb5d6a9b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:37:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:38:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:38:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:38:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:38:41 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:38:43 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:38:44 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:38:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:38:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:38:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:38:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:38:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:38:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:38:54 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:38:55 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:39:49 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:39:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068d235fdc3605555e5f5f986d759f521d9fc2671fc912abe8901595d45d60ab`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a8c13b430e11f8559e49a7516ea0a3df917cf370a512811b24aa6df83f5f0`  
		Last Modified: Wed, 10 Mar 2021 21:45:54 GMT  
		Size: 21.9 MB (21890337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9f0a0d089389068aacce76a6586d1f849ebaf9deb2c0844d2f97c5b1902c3c`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff1be978ab7b3c0c69146b26b6a288d85f12c47eee96ac71cf6a7151566078`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e262b01df5d3b0cf7f18456e428addd58277b7ec59681df285c56631bd530c1f`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeff2c1d9364727bbb7a1de68846e419d9f653f5319da7efbaa323658c26b48`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dad64a77e48bef36bd455f70d9ad06b83544f388bcd8235c25080d45ae8970`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0239d3fcf5f548af5b0c3e7117effa43baef43188cd5a77f063d85387b1d9df`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc76feb0f670cf8be35090ebebe3c4643fa107f237656ca352b95f635993fca`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dee0f2604aa4735cb4916b33c70ea425fa47fdcf149332ff05a43279861bda`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0d846b47ba13cb71b100d80357ad7dc9df41e5baf3f9d9521c42612e609d0b`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2470c6dc6014a45e42ff9f92c2727e721495efd2b9589a5ac5c6f0b22c36490a`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e53076fc5ab0c6120d49ae633dd65d6a0c5a0e0f0e8b708e9e135a12554f067`  
		Last Modified: Wed, 10 Mar 2021 21:45:41 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b9bf97f40f7208eb4539982865006e193756f28a3c7465053d45a8d04c40b4`  
		Last Modified: Wed, 10 Mar 2021 21:45:41 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293df8564c0989a8e85113cf1a8bfdb517a8f6490b5aa9c2e35960aea24bf363`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1870d93517098ab98b14710fa207f6b05ef1366f8bcea48882f0d3baa7abc4`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac094dadecb74c0eb1d8562e2974563f9e7bb5f5dc047f11ec504530cc1a9f14`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ba123c5815bf1a003074b6a7fd124d45546d9807c1e03832c898f388970ae1`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 256.9 KB (256897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6008b4f137610cb112001da1d9980c6fe7689bbdbe6aae8aaf981ed841244e3`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2cd37377aa42041050b07ba0576bbec71e235f9dc11bd2b83a705c9ae38d1ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.4.0-beta.1-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:6e5d5fea5cb01c12f4a392581b1d7cd9c8d057edf35421f107831ac987426788
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487833197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d9298e9342ee167543a1f5ea16eb3acde3c3e78c807d7d27b76ed6bc7587f9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:35:55 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:36:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:36:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:36:28 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:36:29 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:36:31 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:36:32 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:36:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:36:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:36:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:36:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:36:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:36:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:36:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:36:40 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:36:41 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:36:42 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:37:01 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:37:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc803029bd3ef109ba5043ff19061940f4d933b3b12efaadce4d958fff6984b`  
		Last Modified: Wed, 10 Mar 2021 21:45:26 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e23f022464526cb08cf5ae2524d4194aeb092d552b2a12309a02e731b92f2d`  
		Last Modified: Wed, 10 Mar 2021 21:45:30 GMT  
		Size: 16.5 MB (16480793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4417b70d9203a0f38da3e90189d96fca91c20a89c9f840dc3bf64b4f2561ae5c`  
		Last Modified: Wed, 10 Mar 2021 21:45:26 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4755067618a3cdc748f363c5f1a3da8eef0324233e5927f7dbac370b44bdc0`  
		Last Modified: Wed, 10 Mar 2021 21:45:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a4666bc7b476eb9b14bea25d19716eabf278bcba06df2e012e67a38477aa6`  
		Last Modified: Wed, 10 Mar 2021 21:45:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1c2bc1c49e7b0cba9e9ca161fc75374d674e2149ea25c38cf3ceeb9ce2cd5c`  
		Last Modified: Wed, 10 Mar 2021 21:45:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8c6b745994cb1e2bf9dcd0d2819313119ebc53c3fe9b49cdae27bad55cd4ab`  
		Last Modified: Wed, 10 Mar 2021 21:45:23 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0539021a8993cee20a823ee8225ec8615125fa5e331639602e11912f8a3e03c2`  
		Last Modified: Wed, 10 Mar 2021 21:45:24 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dbc014cc64499a05b9a2c7672e407fcf64a2c92e931fb4459f0a576d56d5fd`  
		Last Modified: Wed, 10 Mar 2021 21:45:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1bd855f3e80cdf85c231872b897f41f78624e38bd56da6a854462a3f8f35b4`  
		Last Modified: Wed, 10 Mar 2021 21:45:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2546886727759053cccfd44ac8d85642584457230bdba944f6651dff8ac8bca`  
		Last Modified: Wed, 10 Mar 2021 21:45:20 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2416a88d556dc24e1284df7253ea7257a39f1229564525254f095238f48fc97`  
		Last Modified: Wed, 10 Mar 2021 21:45:20 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ba1c7f3b3b979941d8c0847592ab35f1f82980625a38c804d801b3fa68d7e6`  
		Last Modified: Wed, 10 Mar 2021 21:45:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed032ff3bbe44776ff76827c8edd4ec2164d69d37f472b2127113338b478214f`  
		Last Modified: Wed, 10 Mar 2021 21:45:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783d7b3e5da6311f30234890e25925493d5b34fc2344886a83084492d83f4583`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20049d238f731868cb3d762df8034faf5bc27ba7024494295013a7bdc5782f`  
		Last Modified: Wed, 10 Mar 2021 21:45:18 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c87ab0a491513801045b830deb77e44c71c6eca44368182459f8bf9ccbf94c`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aef85cb3e822cd1c013f9d9cd34377b55595a562fccdeb5829cbe29762d1565`  
		Last Modified: Wed, 10 Mar 2021 21:45:17 GMT  
		Size: 326.1 KB (326117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321fc9e27c48d69216d1c39ccb8e630b835829091e6fec4a070f81b154952691`  
		Last Modified: Wed, 10 Mar 2021 21:45:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:7536cea05647ed76638168e0552a4471d75dbff2a821da4d082f1d576a1abf8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:78fd3e7c57ab3ba12695d70a80262c61da00210106587256cf437f1a9f1e061c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829264967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea8287af00bc3215176603b53641bd1d0bc6a88a00fa2e91b7f469fb5d6a9b2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:37:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:38:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:38:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:38:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:38:41 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:38:43 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:38:44 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 10 Mar 2021 21:38:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:38:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:38:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:38:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:38:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:38:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:38:54 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:38:55 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:39:49 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:39:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068d235fdc3605555e5f5f986d759f521d9fc2671fc912abe8901595d45d60ab`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a8c13b430e11f8559e49a7516ea0a3df917cf370a512811b24aa6df83f5f0`  
		Last Modified: Wed, 10 Mar 2021 21:45:54 GMT  
		Size: 21.9 MB (21890337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9f0a0d089389068aacce76a6586d1f849ebaf9deb2c0844d2f97c5b1902c3c`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff1be978ab7b3c0c69146b26b6a288d85f12c47eee96ac71cf6a7151566078`  
		Last Modified: Wed, 10 Mar 2021 21:45:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e262b01df5d3b0cf7f18456e428addd58277b7ec59681df285c56631bd530c1f`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeff2c1d9364727bbb7a1de68846e419d9f653f5319da7efbaa323658c26b48`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dad64a77e48bef36bd455f70d9ad06b83544f388bcd8235c25080d45ae8970`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0239d3fcf5f548af5b0c3e7117effa43baef43188cd5a77f063d85387b1d9df`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc76feb0f670cf8be35090ebebe3c4643fa107f237656ca352b95f635993fca`  
		Last Modified: Wed, 10 Mar 2021 21:45:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dee0f2604aa4735cb4916b33c70ea425fa47fdcf149332ff05a43279861bda`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0d846b47ba13cb71b100d80357ad7dc9df41e5baf3f9d9521c42612e609d0b`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2470c6dc6014a45e42ff9f92c2727e721495efd2b9589a5ac5c6f0b22c36490a`  
		Last Modified: Wed, 10 Mar 2021 21:45:42 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e53076fc5ab0c6120d49ae633dd65d6a0c5a0e0f0e8b708e9e135a12554f067`  
		Last Modified: Wed, 10 Mar 2021 21:45:41 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b9bf97f40f7208eb4539982865006e193756f28a3c7465053d45a8d04c40b4`  
		Last Modified: Wed, 10 Mar 2021 21:45:41 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293df8564c0989a8e85113cf1a8bfdb517a8f6490b5aa9c2e35960aea24bf363`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1870d93517098ab98b14710fa207f6b05ef1366f8bcea48882f0d3baa7abc4`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac094dadecb74c0eb1d8562e2974563f9e7bb5f5dc047f11ec504530cc1a9f14`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ba123c5815bf1a003074b6a7fd124d45546d9807c1e03832c898f388970ae1`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 256.9 KB (256897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6008b4f137610cb112001da1d9980c6fe7689bbdbe6aae8aaf981ed841244e3`  
		Last Modified: Wed, 10 Mar 2021 21:45:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:30cf6a3da8365c2d9344adfc42b33a5b6e01dc4943c75b0132d556d12bd5f995
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
$ docker pull caddy@sha256:d0b43ebda8fd47409cec98d5f3c3b4c60bfc6bca35338313c002dc64c2283055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88588539bb905b66ad7f78f35b915f2daf56ec49fd5f20019793e9dbd9747497`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:10:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:10:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:10:52 GMT
ENV CADDY_VERSION=v2.3.0
# Sat, 06 Mar 2021 08:10:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:10:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:10:59 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:10:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296b24b4efd312d2a5e0a24a29635cf8aa098c9c3e50ca6566741a54b2794b`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 300.0 KB (300027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0836949366398b595edf3fde04aff8f2a0c0f4c1ea35372e070f4bf27ce59`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7383a05b49b6f752da622ff9a170dccd483a982060cc06a6be10d6312d32a0`  
		Last Modified: Sat, 06 Mar 2021 08:11:52 GMT  
		Size: 11.6 MB (11622385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701a0726354caf82c1c4be1f558173acf8b6604f7b4118a1097b98424256bd`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c03423186b55d3813eb09d04dc53106635be68cfb5969c12109e08cff9aa2cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569b44d4318ddaf5248442e91df11b525d9ccaf230b7efd78c6ce6ef08281ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:07:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:07:11 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:07:11 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:07:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:07:18 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:07:19 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:07:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:07:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:07:26 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:07:27 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:07:28 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:07:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:07:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9d7c4e3e67f9f36b119476dce4a4951c76aca8f9848b7cc600797ce9a5dbb5`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0438df6797a38cba7f30dd40d58d68e90cf6f6a4ece0a3352142ef610796d1`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1886901d622dcb0b11ff563e6eca542fec29b60ae60c1bf82c8d7271fbcb8`  
		Last Modified: Wed, 24 Feb 2021 21:08:13 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f6d93c8b87b0adc5fdfbfb465ceb4e8c5ccbfe7e75288a0b6247b287bd1d19`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35efa62036c16d5ac4716ce79b11c0505538236542b982ce31e580044712c961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e584e1be15b38bc7eddfd01bedf8038c9b6eb1d20a21df121376bc0878fa2b5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:20:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:20:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:20:25 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:20:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:20:32 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:20:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:20:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:20:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:20:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:20:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:20:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:20:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:20:41 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:20:41 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:20:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38341eca332cf74b9be3ce81ca1d45dfb58d85d6d26b7e95c316e6c9bb29ee72`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 299.2 KB (299205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc65ce8d47b334515d1e1114419a952c7a20fde643e2cb7d7fba90886eb905`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dac8b9094b9d9fb88438fba0a9603978bb1779e919ca8adf8673ef932f74e5`  
		Last Modified: Wed, 24 Feb 2021 21:21:23 GMT  
		Size: 10.9 MB (10925347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114ebf580e52effa6a3b734370fc33000e5a7439f0b0b2b275ffaca7483dd32`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9629cb7ae3d67bb1da05e2a4fa565c7549f1d0df99f27e50987ad0414fa275a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0888c16cdeddffbcaf6f274289f92000cb7e408a60c2788e1cecce57fb4f54d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:33:39 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:33:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:33:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:33:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:33:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:33:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:33:49 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:33:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:33:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:33:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:33:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:33:58 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:33:59 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c560f04d39148af03b91ee7707d8a25136794128fdc0eb1a28ee5a9c7ec5`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 300.4 KB (300351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bb894d60771907a615f58e2c0b5873da52637bf52500990e34621581a232d7`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c61561fb1545eb44bb540b09bf7ce497aa3618f51b8dd8013e161cbe6b595d`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d97783fa5ecc238f39ccba3a47e00bbef6ee3ac8db0ad07989b7f65fac81`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:247ebfeff707410bb47d0a0501aee685d43129a4fab344f361ca1430c28a4058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9eef5ad7357ccba137393d95be15feb69c0fb5bf08d5a63bdd1d15f0a957a92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:19:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:19:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:19:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:19:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:19:32 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:19:37 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:19:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:19:40 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866813d62eb8e73b5cfc9e73e48928d678fcad6123ca0697fdc6ff6faf0c91e`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 300.5 KB (300478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8052626100230d16d27888d060e65aaf770add1ae10f69a8f03a903d274ec2`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6a465134a658869ad61a0ea92cf2775ffd82e4cd1d0e2246f24abd0ac95613`  
		Last Modified: Wed, 24 Feb 2021 21:20:17 GMT  
		Size: 11.3 MB (11272060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fffed8a5a7c6c9efd387b3b851eb42ba3b176b5614156a8f2b5ca6dbfe56e7`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:0fb7ab0f5020028979571375f6603af9a59654678c6e4f03ad921a1393b5c243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:862811186da27cadceb66c7ee0cb45d86e6b602f47863023ed8319b3301dbbd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119510533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24e5592ed0aa110ea96dac4d55eefb729afbdc814df500aa6a787dbc57231e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:37:14 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:37:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:37:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:26:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:28:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:28:28 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:28:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:28:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:28:29 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 22:49:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c21a6730e0112f8caa6cdc154b2f867263b01469a8da8db3b07547c4950a2`  
		Last Modified: Sat, 06 Mar 2021 01:46:38 GMT  
		Size: 280.9 KB (280894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f35c144b30bc90da37f39e5fa735d3ece39f8d810a72e602a654f97c14e28`  
		Last Modified: Sat, 06 Mar 2021 01:46:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d74b5e6c1b32d8da263fffffe1571d0aa7840a360e44cef8824e2f92b6fc711`  
		Last Modified: Thu, 11 Mar 2021 22:33:43 GMT  
		Size: 106.8 MB (106807980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ba6a180f195b6f3ec45af31dc20f7f82de4534fa980b59ffaaf3b77d65165`  
		Last Modified: Thu, 11 Mar 2021 22:33:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4a5846e3583aa5bd3bbad43108ab66cec6cad25f06829e8b10f0d224c15d5`  
		Last Modified: Thu, 11 Mar 2021 22:49:57 GMT  
		Size: 8.3 MB (8310380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8a6abbe5760db7bc9db1db175757935f89f61a0423693ac14c3f91da46abf`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007277fd96ef5c07c805416c73c421afa2999ef84692cbb110e791074063bd12`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c4d0afa340d0e2aa233f8278507aee670023b17b80e590c91d93ef3439de448a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef488fb8def86e1b06487105f395f6fc0a7e087069583f3e431d84bcaae2299`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:02:48 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:05:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:05:39 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:05:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:05:43 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:24:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:24:42 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:24:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:24:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:24:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:24:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:24:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614262833bc8b0fc7ca4f64867b162339accb9d3582c54741d8b49f2c64c09`  
		Last Modified: Thu, 11 Mar 2021 23:08:57 GMT  
		Size: 102.7 MB (102672225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bf2e189cc80b997303b9f227dc8e23de317a042c70a3acca6d8b3788e25aa`  
		Last Modified: Thu, 11 Mar 2021 23:08:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f119c8bfefc5869514223494c22fc23a2d68fc033ee20fedc4b3b174415b76b`  
		Last Modified: Thu, 11 Mar 2021 23:25:39 GMT  
		Size: 7.9 MB (7929405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f4de46b783da3ec5fd21ce4bc46ab92cc63fcdc40618084b1adfc1aba00098`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37870025a40d2ec9d941fcb6204cf69ec8d6772a24b7db7d5db1117781a73d25`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:62667b3a24dd819b71004cb01749b845967c223df5ea625100b41ac3d05e2555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113517439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff54e412af0413f30546b8c74fd8c8be5dbea282237684fb43f71203f2175f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:11:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:13:21 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:13:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:13:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:13:26 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:09 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:10 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:58:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd218a9c9cdf2a32d61b9caeabf05fc557d18aba19567001281413ccc166abb6`  
		Last Modified: Thu, 11 Mar 2021 23:19:59 GMT  
		Size: 102.5 MB (102463603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643306f8eda660cb353e21fe422f75cede99a6c613e960ee2286bc348e8176c`  
		Last Modified: Thu, 11 Mar 2021 23:19:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5f28f428a315bb1f0a9910ebcc1381a83256a56de2e96d61f352ee103e3a9`  
		Last Modified: Thu, 11 Mar 2021 23:59:09 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0a908c65e06d906c5f8352e6430d08d7c9dc1b7dc59a5c291fa66e59aa7e6`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 1.2 MB (1219448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e242abfb42c9c0e708ed52f02bc92c3512595611a1ffcf57ff9cef9d3c394f2`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2082102b6f25fc889876abd33fb7f22883f7bb2e2bce98d8a6034fadb887cf26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ede628fb1a9cfec8f6105c863950f2b5ac5e75252b33cf6a2a05f6bbb57d641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:49:25 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:51:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:51:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:51:27 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:13 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6aafe1b0e31e65c7529ef8d21847b8c1efe056cdcd4fbee6ce827c8a6f80e`  
		Last Modified: Thu, 11 Mar 2021 22:57:06 GMT  
		Size: 102.1 MB (102142762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac1f4721e7976668b36bf40054f4c21e6c868baef018741d21154a99b824f6`  
		Last Modified: Thu, 11 Mar 2021 22:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9845f269e96f38704961fb343cccbba5ce6ff2061a46d2ef294070700edbdd62`  
		Last Modified: Thu, 11 Mar 2021 23:14:19 GMT  
		Size: 8.5 MB (8500022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a957bca51081628082676c05f573ad37667ba4ba87785e3e73197652b7358f`  
		Last Modified: Thu, 11 Mar 2021 23:14:14 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3c4fc1979a993abfec003c90073b87df4264100f18e36620b92953459cde3a`  
		Last Modified: Thu, 11 Mar 2021 23:14:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:83e551e622cb784fb7771f8d614a283626c40214db727d7dea05ac64a8a22966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113984663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d7b1fee3cf2dbef32e9959f80faccc3e466774dbd16ea3ab14918fd6a86609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:22:20 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 12 Mar 2021 00:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:24:30 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:24:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:25:09 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:51:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:51:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:51:55 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:52:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:52:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:52:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:52:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2154d5a1378fc4fbd5545832a4424cc2e5dd3613165269dff45cc20e243032fb`  
		Last Modified: Fri, 12 Mar 2021 00:35:25 GMT  
		Size: 100.8 MB (100802905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57651c1165a6ece6782264b696e85781759407e02c29456a701c0fcd2ee66bec`  
		Last Modified: Fri, 12 Mar 2021 00:35:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf1475a468d7b95375a09ed37f89ee94fee4790a3994ddf52921881a7344172`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 8.9 MB (8921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e317bfdf0439372547a8ace4172d14ae9ec69b87a6aebae08ef2e3399f79d3a`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d267f6d8a55227241eb5b4887182e8235cafdfffe5dff7669c5576540b390cac`  
		Last Modified: Fri, 12 Mar 2021 00:54:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:1cc96e1e2875dd10ee3630e1fedf90665895a48e5a75ca4611dfcdf4faaab916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118386946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c72d03c0317c0c4b8c9d6d05ba0f3e4a5389e0d974948f958748fade2ecfa6a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:26:20 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:26:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:26:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:53:49 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:53:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:53:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:53:51 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:46 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ce93a9515faa8483031cd7ac348bce59b30f557f40b533df9e52c358a19e5`  
		Last Modified: Wed, 24 Feb 2021 21:32:29 GMT  
		Size: 281.3 KB (281347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c08039d2964dbc395a13ddd93f041bfb0b0baeae68502ad855f2275c19cdf`  
		Last Modified: Wed, 24 Feb 2021 21:32:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21498377e25a1a2541581a496a9f9201de39caedc60865734db766646a4c8af2`  
		Last Modified: Thu, 11 Mar 2021 22:58:04 GMT  
		Size: 105.9 MB (105920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b19d5e0ba58e1f0c5cf765952f6b60d368718d527771478ca9b28247802316`  
		Last Modified: Thu, 11 Mar 2021 22:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8774f2ce3d2f37a1517d768246eedf3261c9857937f22325c23e630dcab4b`  
		Last Modified: Thu, 11 Mar 2021 23:14:37 GMT  
		Size: 8.4 MB (8352751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c425cbaf74b50e11b534aa5373a068938bf6757dbe03de2347fec50d2c725a`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 1.3 MB (1264422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccdb72140ea082b64ecde8f58d6a55f783edf2f3862bf153e8f985fdb8d9163`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:b479ee29fc292927412fd406cbd98213c86297827a1394d0330aeb893389ca2b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997779833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d39182d3209e4aaf523a2af875e851b8f76036d6c06fb20c6f7fcec6b5513a7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:29:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:33:04 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:33:06 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:06:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:06:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8494855cd5caf3e189463c5ccb6b39747780c1badc12b700373d09d3eda5951`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d01c5a4b0a72580926ec7ca31a0854e4579fc963e0ac611647baf0114f2a66`  
		Last Modified: Thu, 11 Mar 2021 23:45:43 GMT  
		Size: 143.9 MB (143920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50820dad888490de695910927761a6f39cc9279dd81fe9a5c9e6c9251898981a`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dfd1807d2f148f94a7a3347aaf549f9dbc2f2579f0f79923f1f5af98f0b391`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe53f39ec665d626ef91d032f7fd89585e43fc33ccd8683ac6702a9d9e48e2`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5ba9ef95c5e7d8a7b67707b0684405b788b8b40981ecb630f594aa5c2e441`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aff9b53d22053a11e663aac9f51af62d7f29b0f7f6f0796b1bf806f4964f6b`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a037fab4795a44a74e89abfc519243a3cad9ed7e5d5c0109040ff2a2bb457c4`  
		Last Modified: Fri, 12 Mar 2021 00:10:28 GMT  
		Size: 11.5 MB (11517051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f94242e8b9b89dc3a91c2e504dcae074ad187dded384b87b8cf4c29ca92f`  
		Last Modified: Fri, 12 Mar 2021 00:10:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:ab06d627ea66c5536a8cb97a86b3dfed587b811dc803c42dd5fdd65b4255e303
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
$ docker pull caddy@sha256:862811186da27cadceb66c7ee0cb45d86e6b602f47863023ed8319b3301dbbd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119510533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24e5592ed0aa110ea96dac4d55eefb729afbdc814df500aa6a787dbc57231e1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:37:14 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 06 Mar 2021 01:37:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:37:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:26:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:28:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:28:28 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:28:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:28:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:28:29 GMT
WORKDIR /go
# Thu, 11 Mar 2021 22:49:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 22:49:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 22:49:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 22:49:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 22:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 22:49:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 22:49:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c21a6730e0112f8caa6cdc154b2f867263b01469a8da8db3b07547c4950a2`  
		Last Modified: Sat, 06 Mar 2021 01:46:38 GMT  
		Size: 280.9 KB (280894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f35c144b30bc90da37f39e5fa735d3ece39f8d810a72e602a654f97c14e28`  
		Last Modified: Sat, 06 Mar 2021 01:46:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d74b5e6c1b32d8da263fffffe1571d0aa7840a360e44cef8824e2f92b6fc711`  
		Last Modified: Thu, 11 Mar 2021 22:33:43 GMT  
		Size: 106.8 MB (106807980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ba6a180f195b6f3ec45af31dc20f7f82de4534fa980b59ffaaf3b77d65165`  
		Last Modified: Thu, 11 Mar 2021 22:33:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c4a5846e3583aa5bd3bbad43108ab66cec6cad25f06829e8b10f0d224c15d5`  
		Last Modified: Thu, 11 Mar 2021 22:49:57 GMT  
		Size: 8.3 MB (8310380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8a6abbe5760db7bc9db1db175757935f89f61a0423693ac14c3f91da46abf`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007277fd96ef5c07c805416c73c421afa2999ef84692cbb110e791074063bd12`  
		Last Modified: Thu, 11 Mar 2021 22:49:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c4d0afa340d0e2aa233f8278507aee670023b17b80e590c91d93ef3439de448a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef488fb8def86e1b06487105f395f6fc0a7e087069583f3e431d84bcaae2299`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:02:48 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:05:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:05:39 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:05:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:05:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:05:43 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:24:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:24:42 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:24:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:24:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:24:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:24:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:24:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614262833bc8b0fc7ca4f64867b162339accb9d3582c54741d8b49f2c64c09`  
		Last Modified: Thu, 11 Mar 2021 23:08:57 GMT  
		Size: 102.7 MB (102672225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bf2e189cc80b997303b9f227dc8e23de317a042c70a3acca6d8b3788e25aa`  
		Last Modified: Thu, 11 Mar 2021 23:08:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f119c8bfefc5869514223494c22fc23a2d68fc033ee20fedc4b3b174415b76b`  
		Last Modified: Thu, 11 Mar 2021 23:25:39 GMT  
		Size: 7.9 MB (7929405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f4de46b783da3ec5fd21ce4bc46ab92cc63fcdc40618084b1adfc1aba00098`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37870025a40d2ec9d941fcb6204cf69ec8d6772a24b7db7d5db1117781a73d25`  
		Last Modified: Thu, 11 Mar 2021 23:25:37 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:62667b3a24dd819b71004cb01749b845967c223df5ea625100b41ac3d05e2555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113517439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff54e412af0413f30546b8c74fd8c8be5dbea282237684fb43f71203f2175f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:11:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 23:13:21 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 23:13:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 23:13:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 23:13:26 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:58:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:58:09 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:58:10 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:58:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:58:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:58:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:58:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd218a9c9cdf2a32d61b9caeabf05fc557d18aba19567001281413ccc166abb6`  
		Last Modified: Thu, 11 Mar 2021 23:19:59 GMT  
		Size: 102.5 MB (102463603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e643306f8eda660cb353e21fe422f75cede99a6c613e960ee2286bc348e8176c`  
		Last Modified: Thu, 11 Mar 2021 23:19:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5f28f428a315bb1f0a9910ebcc1381a83256a56de2e96d61f352ee103e3a9`  
		Last Modified: Thu, 11 Mar 2021 23:59:09 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0a908c65e06d906c5f8352e6430d08d7c9dc1b7dc59a5c291fa66e59aa7e6`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 1.2 MB (1219448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e242abfb42c9c0e708ed52f02bc92c3512595611a1ffcf57ff9cef9d3c394f2`  
		Last Modified: Thu, 11 Mar 2021 23:59:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2082102b6f25fc889876abd33fb7f22883f7bb2e2bce98d8a6034fadb887cf26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ede628fb1a9cfec8f6105c863950f2b5ac5e75252b33cf6a2a05f6bbb57d641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:49:25 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:51:23 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:51:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:51:27 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:13 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6aafe1b0e31e65c7529ef8d21847b8c1efe056cdcd4fbee6ce827c8a6f80e`  
		Last Modified: Thu, 11 Mar 2021 22:57:06 GMT  
		Size: 102.1 MB (102142762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac1f4721e7976668b36bf40054f4c21e6c868baef018741d21154a99b824f6`  
		Last Modified: Thu, 11 Mar 2021 22:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9845f269e96f38704961fb343cccbba5ce6ff2061a46d2ef294070700edbdd62`  
		Last Modified: Thu, 11 Mar 2021 23:14:19 GMT  
		Size: 8.5 MB (8500022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a957bca51081628082676c05f573ad37667ba4ba87785e3e73197652b7358f`  
		Last Modified: Thu, 11 Mar 2021 23:14:14 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3c4fc1979a993abfec003c90073b87df4264100f18e36620b92953459cde3a`  
		Last Modified: Thu, 11 Mar 2021 23:14:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:83e551e622cb784fb7771f8d614a283626c40214db727d7dea05ac64a8a22966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113984663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d7b1fee3cf2dbef32e9959f80faccc3e466774dbd16ea3ab14918fd6a86609`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:22:20 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 12 Mar 2021 00:24:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 12 Mar 2021 00:24:30 GMT
ENV GOPATH=/go
# Fri, 12 Mar 2021 00:24:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 00:24:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Mar 2021 00:25:09 GMT
WORKDIR /go
# Fri, 12 Mar 2021 00:51:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 12 Mar 2021 00:51:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:51:55 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:52:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:52:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 12 Mar 2021 00:52:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 12 Mar 2021 00:52:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2154d5a1378fc4fbd5545832a4424cc2e5dd3613165269dff45cc20e243032fb`  
		Last Modified: Fri, 12 Mar 2021 00:35:25 GMT  
		Size: 100.8 MB (100802905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57651c1165a6ece6782264b696e85781759407e02c29456a701c0fcd2ee66bec`  
		Last Modified: Fri, 12 Mar 2021 00:35:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf1475a468d7b95375a09ed37f89ee94fee4790a3994ddf52921881a7344172`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 8.9 MB (8921448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e317bfdf0439372547a8ace4172d14ae9ec69b87a6aebae08ef2e3399f79d3a`  
		Last Modified: Fri, 12 Mar 2021 00:54:05 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d267f6d8a55227241eb5b4887182e8235cafdfffe5dff7669c5576540b390cac`  
		Last Modified: Fri, 12 Mar 2021 00:54:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1cc96e1e2875dd10ee3630e1fedf90665895a48e5a75ca4611dfcdf4faaab916
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118386946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c72d03c0317c0c4b8c9d6d05ba0f3e4a5389e0d974948f958748fade2ecfa6a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:26:20 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:26:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:26:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:51:51 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 22:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 11 Mar 2021 22:53:49 GMT
ENV GOPATH=/go
# Thu, 11 Mar 2021 22:53:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 22:53:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 11 Mar 2021 22:53:51 GMT
WORKDIR /go
# Thu, 11 Mar 2021 23:13:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 11 Mar 2021 23:13:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 11 Mar 2021 23:13:46 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 11 Mar 2021 23:13:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 Mar 2021 23:13:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 Mar 2021 23:13:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 Mar 2021 23:13:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ce93a9515faa8483031cd7ac348bce59b30f557f40b533df9e52c358a19e5`  
		Last Modified: Wed, 24 Feb 2021 21:32:29 GMT  
		Size: 281.3 KB (281347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c08039d2964dbc395a13ddd93f041bfb0b0baeae68502ad855f2275c19cdf`  
		Last Modified: Wed, 24 Feb 2021 21:32:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21498377e25a1a2541581a496a9f9201de39caedc60865734db766646a4c8af2`  
		Last Modified: Thu, 11 Mar 2021 22:58:04 GMT  
		Size: 105.9 MB (105920395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b19d5e0ba58e1f0c5cf765952f6b60d368718d527771478ca9b28247802316`  
		Last Modified: Thu, 11 Mar 2021 22:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc8774f2ce3d2f37a1517d768246eedf3261c9857937f22325c23e630dcab4b`  
		Last Modified: Thu, 11 Mar 2021 23:14:37 GMT  
		Size: 8.4 MB (8352751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c425cbaf74b50e11b534aa5373a068938bf6757dbe03de2347fec50d2c725a`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 1.3 MB (1264422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccdb72140ea082b64ecde8f58d6a55f783edf2f3862bf153e8f985fdb8d9163`  
		Last Modified: Thu, 11 Mar 2021 23:14:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f51cbb2f6355b4ba86c8133c76ec964e0385fd4a3ee980a35a7e700ebf761366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:c5137e7e96b3bab8e8fc576b0b43b053f2b1ffe0987ff91247b16292d16391a6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636695753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e648ba82d2c439da46e0294eaa940761c0ea3b3659a842625b35447a33e29451`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:37:21 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:37:22 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:37:23 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:37:24 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:38:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:38:56 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:39:22 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:26:08 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:28:44 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:28:46 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:10 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:11 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:04:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:04:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f55c0bb3b38761f0aaeef923efdf23ab140f64a5549388e9aa125fe79780b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312e589b5b4b52c93afc65c4053591faf5d602a159699e1d8fd7cb7257a1e19`  
		Last Modified: Wed, 10 Mar 2021 14:02:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a36351186e9a8092baf10dfbdfd28b7dce39bcb5b543246f650bf4ad9549d6`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf84abeceee0a3b5a380cf6aa46e231424d48c1781e88f7f96344fdd400753`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcb0c1de08b3116c910ff0e9573389536913cddb0462da67f13cc24f09b479b`  
		Last Modified: Wed, 10 Mar 2021 14:02:55 GMT  
		Size: 34.5 MB (34540168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121ca5c84aae657554fc278543816ed7a73aa34867b296c486181ff025bde056`  
		Last Modified: Wed, 10 Mar 2021 14:02:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1fde90e4880470a95a23f5277f201512a5e7cad1fc6c1bf100e06df43201b0`  
		Last Modified: Wed, 10 Mar 2021 14:02:44 GMT  
		Size: 338.8 KB (338777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0333f27a2b79cd3bdd49673dab866734b9295038aeff265dd3f0ecf22775f450`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8aacb4c9374e105e1433b3bb060fa1422080e3810f669f16525cb18e0e38e4`  
		Last Modified: Thu, 11 Mar 2021 23:42:41 GMT  
		Size: 138.5 MB (138534086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dfe01656430b2cc1a572ee7753450e57326425d287a749250605f446ad6c1`  
		Last Modified: Thu, 11 Mar 2021 23:42:11 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fd43612cf7c7bc62c02a63ab27844b67922e047203f88cd9da8b5f190274d`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4183217b53dd5d304a86da69248467a610c127a01d52afaccd763f665523ece`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b2950f0c1ae60e41816bcd9affab254ecd2dd89c80c8d8d010244ded04572`  
		Last Modified: Fri, 12 Mar 2021 00:09:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8788d1354a7c6deaf4cb2c7159814f8b59023caa733a094dfd4ef5a754f0fd8`  
		Last Modified: Fri, 12 Mar 2021 00:09:55 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e72cb31e323dad57a165b1e6bfe04d758594015a61c8be8b79dcf48612feda`  
		Last Modified: Fri, 12 Mar 2021 00:09:53 GMT  
		Size: 1.7 MB (1729540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e35960d07fabceedb257d51f7d5856daef3fd1fd88096d60cb102c20dc6d3c`  
		Last Modified: Fri, 12 Mar 2021 00:09:52 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:0618e3b1bf17154fccafda7e15f9cd3a661e3515ce15e32f578db0fbb8cb4ede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:b479ee29fc292927412fd406cbd98213c86297827a1394d0330aeb893389ca2b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997779833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d39182d3209e4aaf523a2af875e851b8f76036d6c06fb20c6f7fcec6b5513a7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:42:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Mar 2021 13:42:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Mar 2021 13:42:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Mar 2021 13:42:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Mar 2021 13:44:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 13:44:32 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Mar 2021 13:45:47 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Mar 2021 23:29:06 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 11 Mar 2021 23:33:04 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ba30d211e96d57ce2becf17fe9ebe1d958eba29384c5aeb1e99f9209b44dd7c2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 11 Mar 2021 23:33:06 GMT
WORKDIR C:\gopath
# Fri, 12 Mar 2021 00:04:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 12 Mar 2021 00:04:47 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 12 Mar 2021 00:04:48 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 12 Mar 2021 00:04:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 12 Mar 2021 00:06:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 12 Mar 2021 00:06:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2092de86b10f822dfd3a0d8e8dc35924823393cf8301e6db8f8a0a2879fb18`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ac6e05dba1a284b10130ada4ed7581f5a1c5a90986038e31cc8213e215ca23`  
		Last Modified: Wed, 10 Mar 2021 14:06:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636ee1e87a6b10caeaef03b68f084d58b5c8412fe4b10ba5d851a6965917196`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e03ef5102108f3595c37759ead10b0cfb624aa0f102dbae3b6abb18f03b56`  
		Last Modified: Wed, 10 Mar 2021 14:06:01 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840634d0d343cc458ff1f028b165fab14415bf252ce2b7fdb726c41d035c64ff`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 35.3 MB (35273703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b968b2b2cb37afe5893ed1aa040b1055605f41e8371fe42fca9c6e06bb96c2ed`  
		Last Modified: Wed, 10 Mar 2021 14:05:55 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01350c0465bbc3ff96b788fef94740af9378a1cfe9f3c1fb50ffed30c8a7ad`  
		Last Modified: Wed, 10 Mar 2021 14:05:59 GMT  
		Size: 10.1 MB (10139029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8494855cd5caf3e189463c5ccb6b39747780c1badc12b700373d09d3eda5951`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d01c5a4b0a72580926ec7ca31a0854e4579fc963e0ac611647baf0114f2a66`  
		Last Modified: Thu, 11 Mar 2021 23:45:43 GMT  
		Size: 143.9 MB (143920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50820dad888490de695910927761a6f39cc9279dd81fe9a5c9e6c9251898981a`  
		Last Modified: Thu, 11 Mar 2021 23:42:55 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dfd1807d2f148f94a7a3347aaf549f9dbc2f2579f0f79923f1f5af98f0b391`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe53f39ec665d626ef91d032f7fd89585e43fc33ccd8683ac6702a9d9e48e2`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5ba9ef95c5e7d8a7b67707b0684405b788b8b40981ecb630f594aa5c2e441`  
		Last Modified: Fri, 12 Mar 2021 00:10:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0aff9b53d22053a11e663aac9f51af62d7f29b0f7f6f0796b1bf806f4964f6b`  
		Last Modified: Fri, 12 Mar 2021 00:10:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a037fab4795a44a74e89abfc519243a3cad9ed7e5d5c0109040ff2a2bb457c4`  
		Last Modified: Fri, 12 Mar 2021 00:10:28 GMT  
		Size: 11.5 MB (11517051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f94242e8b9b89dc3a91c2e504dcae074ad187dded384b87b8cf4c29ca92f`  
		Last Modified: Fri, 12 Mar 2021 00:10:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:9485932040de498b47cf0b6cc5d23cbbfd6282e5ff4884b04413cfda0e642661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:d0b43ebda8fd47409cec98d5f3c3b4c60bfc6bca35338313c002dc64c2283055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88588539bb905b66ad7f78f35b915f2daf56ec49fd5f20019793e9dbd9747497`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 08:10:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 06 Mar 2021 08:10:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Sat, 06 Mar 2021 08:10:52 GMT
ENV CADDY_VERSION=v2.3.0
# Sat, 06 Mar 2021 08:10:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 06 Mar 2021 08:10:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 06 Mar 2021 08:10:56 GMT
ENV XDG_DATA_HOME=/data
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/config]
# Sat, 06 Mar 2021 08:10:57 GMT
VOLUME [/data]
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 06 Mar 2021 08:10:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 06 Mar 2021 08:10:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 80
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 443
# Sat, 06 Mar 2021 08:10:59 GMT
EXPOSE 2019
# Sat, 06 Mar 2021 08:10:59 GMT
WORKDIR /srv
# Sat, 06 Mar 2021 08:10:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296b24b4efd312d2a5e0a24a29635cf8aa098c9c3e50ca6566741a54b2794b`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 300.0 KB (300027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0836949366398b595edf3fde04aff8f2a0c0f4c1ea35372e070f4bf27ce59`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7383a05b49b6f752da622ff9a170dccd483a982060cc06a6be10d6312d32a0`  
		Last Modified: Sat, 06 Mar 2021 08:11:52 GMT  
		Size: 11.6 MB (11622385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701a0726354caf82c1c4be1f558173acf8b6604f7b4118a1097b98424256bd`  
		Last Modified: Sat, 06 Mar 2021 08:11:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c03423186b55d3813eb09d04dc53106635be68cfb5969c12109e08cff9aa2cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569b44d4318ddaf5248442e91df11b525d9ccaf230b7efd78c6ce6ef08281ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:07:08 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:07:11 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:07:11 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:07:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:07:18 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:07:19 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:07:20 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:07:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:07:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:07:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:07:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:07:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:07:26 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:07:27 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:07:28 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:07:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:07:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9d7c4e3e67f9f36b119476dce4a4951c76aca8f9848b7cc600797ce9a5dbb5`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 300.1 KB (300107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0438df6797a38cba7f30dd40d58d68e90cf6f6a4ece0a3352142ef610796d1`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1886901d622dcb0b11ff563e6eca542fec29b60ae60c1bf82c8d7271fbcb8`  
		Last Modified: Wed, 24 Feb 2021 21:08:13 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f6d93c8b87b0adc5fdfbfb465ceb4e8c5ccbfe7e75288a0b6247b287bd1d19`  
		Last Modified: Wed, 24 Feb 2021 21:08:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35efa62036c16d5ac4716ce79b11c0505538236542b982ce31e580044712c961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e584e1be15b38bc7eddfd01bedf8038c9b6eb1d20a21df121376bc0878fa2b5e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:20:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:20:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:20:25 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:20:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:20:31 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:20:32 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:20:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:20:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:20:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:20:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:20:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:20:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:20:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:20:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:20:40 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:20:41 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:20:41 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:20:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38341eca332cf74b9be3ce81ca1d45dfb58d85d6d26b7e95c316e6c9bb29ee72`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 299.2 KB (299205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dc65ce8d47b334515d1e1114419a952c7a20fde643e2cb7d7fba90886eb905`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dac8b9094b9d9fb88438fba0a9603978bb1779e919ca8adf8673ef932f74e5`  
		Last Modified: Wed, 24 Feb 2021 21:21:23 GMT  
		Size: 10.9 MB (10925347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114ebf580e52effa6a3b734370fc33000e5a7439f0b0b2b275ffaca7483dd32`  
		Last Modified: Wed, 24 Feb 2021 21:21:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9629cb7ae3d67bb1da05e2a4fa565c7549f1d0df99f27e50987ad0414fa275a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0888c16cdeddffbcaf6f274289f92000cb7e408a60c2788e1cecce57fb4f54d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:33:39 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:33:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:33:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:33:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:33:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:33:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:33:49 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:33:50 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:33:51 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:33:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:33:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:33:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:33:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:33:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:33:57 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:33:58 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:33:59 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:34:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c560f04d39148af03b91ee7707d8a25136794128fdc0eb1a28ee5a9c7ec5`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 300.4 KB (300351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bb894d60771907a615f58e2c0b5873da52637bf52500990e34621581a232d7`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c61561fb1545eb44bb540b09bf7ce497aa3618f51b8dd8013e161cbe6b595d`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d97783fa5ecc238f39ccba3a47e00bbef6ee3ac8db0ad07989b7f65fac81`  
		Last Modified: Wed, 24 Feb 2021 21:34:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:247ebfeff707410bb47d0a0501aee685d43129a4fab344f361ca1430c28a4058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9eef5ad7357ccba137393d95be15feb69c0fb5bf08d5a63bdd1d15f0a957a92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:19:19 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:19:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:19:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:19:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:19:31 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:19:32 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:19:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:19:37 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:19:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:19:40 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866813d62eb8e73b5cfc9e73e48928d678fcad6123ca0697fdc6ff6faf0c91e`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 300.5 KB (300478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8052626100230d16d27888d060e65aaf770add1ae10f69a8f03a903d274ec2`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6a465134a658869ad61a0ea92cf2775ffd82e4cd1d0e2246f24abd0ac95613`  
		Last Modified: Wed, 24 Feb 2021 21:20:17 GMT  
		Size: 11.3 MB (11272060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fffed8a5a7c6c9efd387b3b851eb42ba3b176b5614156a8f2b5ca6dbfe56e7`  
		Last Modified: Wed, 24 Feb 2021 21:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:0d7ec2ae02e36f8374b028af66afcca548c8995638a733f0ad2e7861e2775e7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:dfa33ff752c331d4b76bfe3817fd42ef3ef0bc24d9167cdfdd39f137054ea298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:971ecb6797495e16d5ee3ede15138f5ceaee0930af2ee0b6fbc9dbae848302fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:e9416497e1d43fd04e244f89af4e210714a28b676cf1e2279487484087b8ee39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829241236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b987ba0d14c06619541f1cb51215c36133a17cfbfea49a9bc79b021564ab785`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:30:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:30:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:32:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:32:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:32:13 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:32:14 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:32:15 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:32:16 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:32:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:32:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:32:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:32:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:32:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:32:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:32:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:32:26 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:32:27 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:32:28 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:33:17 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:33:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c9e18c1004b748968faecba6f9d1b5e6233e7e0b82b1c1259cf945eb3334e6`  
		Last Modified: Wed, 10 Mar 2021 21:44:17 GMT  
		Size: 10.2 MB (10181612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f9c532d82c90ea9fc2e2c6a591988abfb79e551caabead3fe56f8ba69c31f6`  
		Last Modified: Wed, 10 Mar 2021 21:44:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5695a08e71ba7869b2e8b11e6f3f228a8a6d303878131e1f3abdc655757b5f2`  
		Last Modified: Wed, 10 Mar 2021 21:44:19 GMT  
		Size: 21.9 MB (21867123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabb7c4e3c2c8cdeef81bd8a6fcaed6b082e5ea4120a15ae4e277258c03de007`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec41ded5794a348cd9c06286dcbe7ca964197008812567791bc45b22bc4dd1`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ab0530e5214beccbf36a30fe1618f9752274c51a313bb71e9b9b130870164`  
		Last Modified: Wed, 10 Mar 2021 21:44:11 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0a7b2c54a3fa027e26d52abd2013c77fc0e69bf93446d70990dc40a6e00d98`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0051bde2db70124d244a1337ccc824629e18f2be3b800ec577a7794ff1f7f3`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271b14baf3d87c6aa3bd2da952290cec023b40b90b62688c79fa26d9253770ac`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9b324fb71cb6bdc3dfd42355efbd64634f7d2ec678a5a15757e69145f671d`  
		Last Modified: Wed, 10 Mar 2021 21:44:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d93b07db92b46680fe5ba78d29058e6f5b2ce49ba20cb10aeccb751b37d497`  
		Last Modified: Wed, 10 Mar 2021 21:44:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6dc81911c7b01e751b8d5a08f7cf494f5542f166b2e1471a08ef82b4ebcb4`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53bfaf85823badcda6fa4470993f24b9772597b13989ee71ec0b5686be93cbc`  
		Last Modified: Wed, 10 Mar 2021 21:44:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5077aa28e94279b15dbe048f37904704877b5b4a932e67a3a12adf8bdfe9ada`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5851fcb607a8afd06548b48e611020418ed88f0c0e1abcba7854089c8bf9729e`  
		Last Modified: Wed, 10 Mar 2021 21:44:06 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498aa4d3ee4135d0aaeccdf4fe0d8ec98c3ba95a92fd0b56dc73a461be700516`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0651b67304c2388b503cbd386e0235ec00a5a8437a9d115ba871152ae9d07103`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418b36ca2fc9603d0a6a28d6f4849cdfd80c3069ea494baeba2ce37e66b73d4`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50dd910f71fe0ceefc794aaee3e6669cd578ae8286348a76c60dc926778da33`  
		Last Modified: Wed, 10 Mar 2021 21:44:04 GMT  
		Size: 256.4 KB (256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a39a5ecfed250f608279f4544ced05934bd84e326d05f119a12081aa38b39f`  
		Last Modified: Wed, 10 Mar 2021 21:44:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
