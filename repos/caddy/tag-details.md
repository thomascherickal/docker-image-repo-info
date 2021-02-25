<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
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
$ docker pull caddy@sha256:72da1ab397f9f002ad371ff4ae4c4b477a9c9fe73f37e87de981ae4c98986280
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
$ docker pull caddy@sha256:9c7988221ae79035b2451e3747a0ecdd8431be642132626a2d113493d0340f9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2160ea65c1af29529ed745aa66e384c6bf69b6476cb887c7f5c20be899abd260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:01:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:01:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:01:29 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:01:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:01:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:01:35 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:01:36 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:01:38 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:01:39 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:01:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e943fcd90b84a982b5885d766383fe0854ebe777f92c4e607d3ac1410cf06e`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 299.9 KB (299950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bb94c554bfa30e776d58e02f639b022f13f4f8d28f2ea51fe1569d0f3342b`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ec0fb337e64a01607417a0d90cbfa0cf4937a4609bce91892ce3c518332d2`  
		Last Modified: Wed, 24 Feb 2021 21:02:26 GMT  
		Size: 11.6 MB (11622361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0e4e5582798cbcbf63965ea2dac6d5e93471bb0f62074d572c2d9806fcc8`  
		Last Modified: Wed, 24 Feb 2021 21:02:23 GMT  
		Size: 154.0 B  
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

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:72da1ab397f9f002ad371ff4ae4c4b477a9c9fe73f37e87de981ae4c98986280
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
$ docker pull caddy@sha256:9c7988221ae79035b2451e3747a0ecdd8431be642132626a2d113493d0340f9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2160ea65c1af29529ed745aa66e384c6bf69b6476cb887c7f5c20be899abd260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:01:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:01:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:01:29 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:01:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:01:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:01:35 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:01:36 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:01:38 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:01:39 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:01:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e943fcd90b84a982b5885d766383fe0854ebe777f92c4e607d3ac1410cf06e`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 299.9 KB (299950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bb94c554bfa30e776d58e02f639b022f13f4f8d28f2ea51fe1569d0f3342b`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ec0fb337e64a01607417a0d90cbfa0cf4937a4609bce91892ce3c518332d2`  
		Last Modified: Wed, 24 Feb 2021 21:02:26 GMT  
		Size: 11.6 MB (11622361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0e4e5582798cbcbf63965ea2dac6d5e93471bb0f62074d572c2d9806fcc8`  
		Last Modified: Wed, 24 Feb 2021 21:02:23 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:186302fda6b402513edbfe8ff920e13d096d2838b43757ea2718a36ef79a54b8
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
$ docker pull caddy@sha256:9c7988221ae79035b2451e3747a0ecdd8431be642132626a2d113493d0340f9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2160ea65c1af29529ed745aa66e384c6bf69b6476cb887c7f5c20be899abd260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:01:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:01:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:01:29 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:01:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:01:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:01:35 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:01:36 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:01:38 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:01:39 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:01:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e943fcd90b84a982b5885d766383fe0854ebe777f92c4e607d3ac1410cf06e`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 299.9 KB (299950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bb94c554bfa30e776d58e02f639b022f13f4f8d28f2ea51fe1569d0f3342b`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ec0fb337e64a01607417a0d90cbfa0cf4937a4609bce91892ce3c518332d2`  
		Last Modified: Wed, 24 Feb 2021 21:02:26 GMT  
		Size: 11.6 MB (11622361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0e4e5582798cbcbf63965ea2dac6d5e93471bb0f62074d572c2d9806fcc8`  
		Last Modified: Wed, 24 Feb 2021 21:02:23 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:639e197fa1970e89c9466452a95e9701fc3d06ad5f85d4c4cf7fcf51875de656
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
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
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
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
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
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
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
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
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
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
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
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
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
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
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
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
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
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
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
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
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
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
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
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
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
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
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
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
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
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:6847eff581ebbf642621d409c59845c6991e154136045f3ed113b337366bc5d0
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
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
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
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
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
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
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
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
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
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
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
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
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
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
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
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
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
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
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
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
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
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb33c8de1233228709c51b4f60dc46b9c661051664b72b9677728f592fb795c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
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
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
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
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:8e5dcc2f90feef29505c8c129dd01f248bfd711239067688d5e3f62344e0e98a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
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
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
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
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
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

## `caddy:2.4.0-beta.1`

```console
$ docker pull caddy@sha256:dbb361e96f42dcaccad00693be8205cab82c6f5851b2c6b484c43bd55e066626
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

### `caddy:2.4.0-beta.1` - linux; amd64

```console
$ docker pull caddy@sha256:c60526866e626c1bf50664a2ecfb9edc1df6ae7cace08429a17752f6eb4c57fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14763747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:722fc49e7238f90957d7a4bac72435ec42233dbf008fee28e6b92b04ec2ae150`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 19:22:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 19:22:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 19:22:03 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:22:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 19:22:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 19:22:07 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 19:22:07 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 19:22:07 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 19:22:07 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:22:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:22:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:22:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:22:09 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:22:09 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:22:10 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:22:10 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 19:22:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fe9c7ee9658d862ee04bee48cb11b8e5a68e38e809bcb6ccf96826679a4f5b`  
		Last Modified: Wed, 24 Feb 2021 19:22:44 GMT  
		Size: 300.3 KB (300320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b09bc90948c5a9a7e1cbda3553ae2da2f0b1d9602350dcc3df2c7f7e174e18`  
		Last Modified: Wed, 24 Feb 2021 19:22:45 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f70b1ecf8ddd8abb75d5081406ef1f030b724a7b04650c29cdf71cf46355cc`  
		Last Modified: Wed, 24 Feb 2021 19:22:47 GMT  
		Size: 11.6 MB (11645861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eae6f927ba520632f23b7ef7c69b23e22013a26c21266591f6b4152f4be0608`  
		Last Modified: Wed, 24 Feb 2021 19:22:45 GMT  
		Size: 154.0 B  
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

### `caddy:2.4.0-beta.1` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4cdeba0900efe52172abfbcaba09cbf73eb331dd494069ce5d7d3edf60aef105
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465520956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4da660c15226e24c8818c56bcd37329210b1be2f7f7a7685824dd821cf87e4`
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
# Wed, 24 Feb 2021 19:17:36 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:18:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 24 Feb 2021 19:18:07 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 24 Feb 2021 19:18:09 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 24 Feb 2021 19:18:10 GMT
VOLUME [c:/config]
# Wed, 24 Feb 2021 19:18:11 GMT
VOLUME [c:/data]
# Wed, 24 Feb 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:18:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:18:21 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:18:22 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:18:23 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:18:38 GMT
RUN caddy version
# Wed, 24 Feb 2021 19:18:39 GMT
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
	-	`sha256:f329d3bba024566dab2f54071c6fba793f7fc404fc263b3aabb7601c9bf2fb2f`  
		Last Modified: Wed, 24 Feb 2021 19:25:02 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0eee823ef67f2c681b991fe34c0d27d2a44fa8bf09aa82dd505ba02b96cead`  
		Last Modified: Wed, 24 Feb 2021 19:25:06 GMT  
		Size: 16.5 MB (16493289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2210192c57f0a5c9bcbe3ab21f13741fd237b6420b8c670eed14a22a16ee80bb`  
		Last Modified: Wed, 24 Feb 2021 19:24:59 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d3f637f6812bd743380eebe8562e9eceaf5c6f8fccb74dcdfa8c5c155676e`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6704bc8ecdf53603807915f467f051697beb2db554852b9e20ea0ba6e79a2`  
		Last Modified: Wed, 24 Feb 2021 19:24:57 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ba0394b89181a0a2a9f8f4c14cbe4071c17bade6f66e0932dca617c8504bd`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c5104a4e7bc41571751f57783252f586c119a2e53e95224b18b98df981991`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927608485d189dbdd46f2b6a3143e94cb5546ea4d8baaeb31008d8217ab1d10`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d07473d7282ce10d7338969fa4a521267f81eaefaf34bebb643ca2f36c506`  
		Last Modified: Wed, 24 Feb 2021 19:24:53 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886d84a62de83fb3db42795e623d933b7c6d7c060310dfd26a999216c198020`  
		Last Modified: Wed, 24 Feb 2021 19:24:51 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a0c8d74f92a4f3a0cf6010e0a694402535f0e7c9aa7f3c23a43b5658180927`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cbae6a4753f68cc678ccff331d7979824475f16e5347a7f642bb0623366d3`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0076f0ebea58934879757debf312e4720988c27c090a78f2cf86585dc0f2b0`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7a116da5f39e6bb191c00a41dcab7309e8fa3c5c75a1c8cd4a298923db823e`  
		Last Modified: Wed, 24 Feb 2021 19:24:51 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a35eec38e96847beea1ab1041a962421f9da53734c8d2aeda03fe21451ab385`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5ade964bcedfaa3d1305c7630f31fc759157cc72491a8b3b3927bab60e977`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c81a658875f96063212596f9c09e82dd68db7e0bb52595402ae4ada2865ad9`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0b796ca125b226c1c29c71496c5a1909375b96c2ca437586ff519ede12434`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 310.0 KB (310045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefe957f99ec30bdadabfe9d1e567a62f6b9ea7e0a2a823606e07f16466d42c`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:ddaa5a644e0bf998397932e079929ef88eefd667e91007b58db748808ea3753b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827363881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bb9bdf3d216ef29abbd04a4936b94a7287286b88c3d15d550d8a07880e826e`
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
# Wed, 24 Feb 2021 19:18:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:20:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 24 Feb 2021 19:20:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 24 Feb 2021 19:20:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 24 Feb 2021 19:20:13 GMT
VOLUME [c:/config]
# Wed, 24 Feb 2021 19:20:14 GMT
VOLUME [c:/data]
# Wed, 24 Feb 2021 19:20:15 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:20:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:20:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:20:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:20:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:20:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:20:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:20:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:20:24 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:20:25 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:20:26 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:21:07 GMT
RUN caddy version
# Wed, 24 Feb 2021 19:21:08 GMT
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
	-	`sha256:620b960cc16ddec3206afd68382c040b072539c2cf01242c1e4b5a5dfca7d028`  
		Last Modified: Wed, 24 Feb 2021 19:25:27 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a31f0da573a4abd5d0843b1660aa4f5e2ab59b1ec4d8ccf225b1f3d35c597c`  
		Last Modified: Wed, 24 Feb 2021 19:25:48 GMT  
		Size: 21.9 MB (21886898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb06c4c8131855b07a7e6aedf897493c47175ba4dc276d26cfebd4b4098595fb`  
		Last Modified: Wed, 24 Feb 2021 19:25:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dc50f20b45c1477c56f840dc00ef32901efae31ed270d7dd8e8845ca64720b`  
		Last Modified: Wed, 24 Feb 2021 19:25:26 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6703e6122eb70ecd05222f36b06445d6e2c2aefdc019fb5b0341241e652a53`  
		Last Modified: Wed, 24 Feb 2021 19:25:22 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf3790132d185f7e33b7053b6f4dda7c7e28a06b4f1d32854f67a3cd04dccb0`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47157fb5a89d548d92f0b15ec5ec80a9d17c893aea9803ca5a0c0f9219fc6ec0`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e55b1c202dbdf0fe8326434a42ff3595e08e3f9cfde195aa51392db7f28f8`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33ee4c38831d27e736ad2e1c0594afee3d66c737928c5a1d7559845b4e1c28b`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9dd6b6a2798e8046294e2f0f344a10ae3abbde16affc3503250a7a831c5534`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6210a68b0d3529c79c68790765bb978c0670600837a00a1459b9224e0c163bcc`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afdaf4879538ca073c8a1713e8da86b01c686d3a2c0eecf13dab42d42334416`  
		Last Modified: Wed, 24 Feb 2021 19:25:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf56b89756efdcac0787d0e591907289fbbe3b9a52a0a0f23e522407dd06be`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a758a2e5470fa296d7d2502ab3d42444ce8952a1a81d9afcaadb8413355b89`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935097fef5cb53c8029a6d7c1bb86f992eee3b23c3299f1a8c8b7ce4431bef34`  
		Last Modified: Wed, 24 Feb 2021 19:25:15 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271677474997ecda9d71f27b0e98a3e37177ffa4300e7722f43cb4d159105f61`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5843ab6da12a2b587a4cc80bcc23f45340c43cd6b1f654f25b59d9d7ebd4fb7`  
		Last Modified: Wed, 24 Feb 2021 19:25:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d053551a5b55945e305bf63d8ab4bf9b0c6d009c83b05b1e3566f6b2bf04d`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 260.6 KB (260550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970166f3bfb7d87cfcf06548a018973d37f49049b2f451706eecb6d03a98c349`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-alpine`

```console
$ docker pull caddy@sha256:5b70705555fca2080fad13f31c88667cf808db21dda0d756165df25c1f96cbc8
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
$ docker pull caddy@sha256:c60526866e626c1bf50664a2ecfb9edc1df6ae7cace08429a17752f6eb4c57fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14763747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:722fc49e7238f90957d7a4bac72435ec42233dbf008fee28e6b92b04ec2ae150`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 19:22:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 19:22:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 19:22:03 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:22:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 19:22:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 19:22:07 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 19:22:07 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 19:22:07 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 19:22:07 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:22:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:22:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:22:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:22:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:22:09 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:22:09 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:22:10 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:22:10 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 19:22:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fe9c7ee9658d862ee04bee48cb11b8e5a68e38e809bcb6ccf96826679a4f5b`  
		Last Modified: Wed, 24 Feb 2021 19:22:44 GMT  
		Size: 300.3 KB (300320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b09bc90948c5a9a7e1cbda3553ae2da2f0b1d9602350dcc3df2c7f7e174e18`  
		Last Modified: Wed, 24 Feb 2021 19:22:45 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f70b1ecf8ddd8abb75d5081406ef1f030b724a7b04650c29cdf71cf46355cc`  
		Last Modified: Wed, 24 Feb 2021 19:22:47 GMT  
		Size: 11.6 MB (11645861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eae6f927ba520632f23b7ef7c69b23e22013a26c21266591f6b4152f4be0608`  
		Last Modified: Wed, 24 Feb 2021 19:22:45 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:1dda4f28ac5cf495b68f582f4e6827ef9a0e35e6558f78a1b1bb0663c2d73d70
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

### `caddy:2.4.0-beta.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:fb66c744a934e5394fc5f784a2a01e392ee1d4ac871bb7aa73bc53ec44366c46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116485823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ea040656d90666d3f0d3a24d7dffc6c76b95687ca0ec68cd818e56892bc01`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:40:50 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 22:40:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 22:40:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 22:40:51 GMT
ENV GOLANG_VERSION=1.16
# Thu, 25 Feb 2021 04:39:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:39:59 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:39:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:40:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:40:00 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:24 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 25 Feb 2021 05:10:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a078c6c131006663e0108b8cef6955129ece35a6e80457b136ed6aa89e4e11`  
		Last Modified: Wed, 17 Feb 2021 22:51:07 GMT  
		Size: 281.2 KB (281187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f90fd1d94bfeb4d4ed803aed56e7043d6b70c53b2c4abbe8d991d976806ee`  
		Last Modified: Wed, 17 Feb 2021 22:51:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdc4f024afdfc3df10c01e560b5a806ee703b0adf125d232e89ffb4e93dc271`  
		Last Modified: Thu, 25 Feb 2021 04:49:11 GMT  
		Size: 105.7 MB (105693504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b7f786c0727dff7e48f0dd73ffc2e720aa86ce3a3375f2408583d85cd4755a`  
		Last Modified: Thu, 25 Feb 2021 04:48:53 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6ef60a9cbf7b15e2e66c1fe96c2df5ff21ef1e67c2c1b71e87d6937ecefa02`  
		Last Modified: Thu, 25 Feb 2021 05:10:54 GMT  
		Size: 6.4 MB (6387716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9117268777094dec4f2c007e2668dc08fd44f1d444398461654565644e6001`  
		Last Modified: Thu, 25 Feb 2021 05:10:52 GMT  
		Size: 1.3 MB (1311072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8328762831932af440a9a3bb8c34afdef0804dab09132cfbb7973b876d57ad44`  
		Last Modified: Thu, 25 Feb 2021 05:10:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d2b866a0ae711fa875f348fb6417a974ead445204fd5c5a3ea01dbb09a3a5da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112253502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581c9e901c158ef3f74130d144d8f07116224cc9a8719a732e7d8772eceffb08`
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
# Wed, 17 Feb 2021 21:13:48 GMT
ENV GOLANG_VERSION=1.16
# Thu, 25 Feb 2021 03:47:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:48:04 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:48:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:48:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:48:07 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:35:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 25 Feb 2021 04:35:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:35:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:35:08 GMT
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
	-	`sha256:bace9343badd2dadb675a52f16f3ca4ccd112da029eee05d5355e75c0ab4c896`  
		Last Modified: Thu, 25 Feb 2021 03:58:25 GMT  
		Size: 101.9 MB (101903218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5a22f9f0218553919c9ed75b438a84f021bfd75f0fdf31e4606bccd643b73`  
		Last Modified: Thu, 25 Feb 2021 03:48:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f47979b8644c84f4fb66ada27db79035ef367f96c327d01cb9715512220a41`  
		Last Modified: Thu, 25 Feb 2021 04:35:52 GMT  
		Size: 6.2 MB (6224571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda9ebdf27fe5887f1d80c5b1ff2e7e50d4b10f34a18a68a77084595581749d`  
		Last Modified: Thu, 25 Feb 2021 04:35:50 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea394686359ebc055063fd14cdc1f2e1811fb623d6e00dc0e2cbd0336d97c08`  
		Last Modified: Thu, 25 Feb 2021 04:35:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ab4e24de38d7d287168310442ff1608d3289cf1f4eedca5d0ac99674e9563fb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111155980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66a07c48b16e7d8f0feb7c043a34e9ca71d0beeba68bcd923599fa97ece655d`
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
# Wed, 17 Feb 2021 21:40:41 GMT
ENV GOLANG_VERSION=1.16
# Thu, 25 Feb 2021 03:34:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:34:15 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:34:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:34:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:34:19 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:57 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:58 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 25 Feb 2021 04:04:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:04:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:04:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:04:07 GMT
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
	-	`sha256:8b89f1d7fa372cb0e714983a27382a72cd9a5e5f73733b308b2a62f5bb1e3496`  
		Last Modified: Thu, 25 Feb 2021 03:44:43 GMT  
		Size: 101.7 MB (101673489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c84ed09a6a9bd0980324017bfa100dd3e954b188ade04e9e18822b82f18bcf`  
		Last Modified: Thu, 25 Feb 2021 03:44:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93bd526776a73b96e82d27d54ff24510e3d867161d56f4c6f9516ff05b4ce0`  
		Last Modified: Thu, 25 Feb 2021 04:04:44 GMT  
		Size: 5.6 MB (5557907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac831342f93da8aeb2bd524789a3e0622343c77a380b859bae56c5b514737c`  
		Last Modified: Thu, 25 Feb 2021 04:04:43 GMT  
		Size: 1.2 MB (1219449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c0836e37206eaa801b6fa33b09a51a6d781a99fed99103b5df42302ba3618a`  
		Last Modified: Thu, 25 Feb 2021 04:04:43 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:06e2fa7ac82894126d4c59e8ebdb1b3cd35192bd5380628827055df543862103
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111686232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:863624a1a77d720a00482a98e959ecee09e1509f2980e85be0adafb3b3afe501`
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
# Wed, 17 Feb 2021 21:28:34 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 21:30:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 17 Feb 2021 21:30:44 GMT
ENV GOPATH=/go
# Wed, 17 Feb 2021 21:30:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 21:30:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 17 Feb 2021 21:30:50 GMT
WORKDIR /go
# Wed, 24 Feb 2021 18:48:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 18:48:34 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:48:35 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:48:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:48:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:48:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:48:41 GMT
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
	-	`sha256:acb1b01f386a26b11a631443b9b147712664e2b7bb6a08c820259bb6d8dceca5`  
		Last Modified: Wed, 17 Feb 2021 21:34:37 GMT  
		Size: 101.0 MB (101017423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81f77ca7a56bd184d62fd0e65d33077ba482a38e0fa2f128668f9cef65ad766`  
		Last Modified: Wed, 17 Feb 2021 21:34:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c163de3737f8bd6236ce025f7f4620f02a9ffbad6c02df77c7ab1683196de22`  
		Last Modified: Wed, 24 Feb 2021 18:49:32 GMT  
		Size: 6.5 MB (6473491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da6df0249182fed0f9e6c06bf3a2d5328743e1af9d4d16ee374cb5594f5be49`  
		Last Modified: Wed, 24 Feb 2021 18:49:28 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fc6e66c939043b655941a2d5886aa6fb247601ed47205dc157a82f09f1055`  
		Last Modified: Wed, 24 Feb 2021 18:49:28 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7d5aa30a0c0011b1b4432d0b6b49b49991ebb60becf80be59269cefaf1e0336d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110550372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3afc18a2b038a1d7a452c0c571581412432b0adfcfa5176d56fa8c105934fb`
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
# Wed, 17 Feb 2021 22:01:11 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 22:03:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 17 Feb 2021 22:03:52 GMT
ENV GOPATH=/go
# Wed, 17 Feb 2021 22:03:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 22:04:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 17 Feb 2021 22:04:32 GMT
WORKDIR /go
# Wed, 24 Feb 2021 19:56:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 19:56:39 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:56:42 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:56:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:57:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 19:57:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 19:57:22 GMT
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
	-	`sha256:9111591a7eef4253aba30dd3eae45995c334bf7d627ce834dbf79f283fa1bb48`  
		Last Modified: Wed, 17 Feb 2021 22:08:49 GMT  
		Size: 99.5 MB (99460179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d30531ced472075060419d974e043566600f535317ecb701b4183ca3ce76936`  
		Last Modified: Wed, 17 Feb 2021 22:08:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ec9433e8ec8bc30b8d6c1ef4e505c341111ef0430e62a2771ad178d28c19f0`  
		Last Modified: Wed, 24 Feb 2021 19:58:23 GMT  
		Size: 6.8 MB (6822502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0159ae43773b5a368197692ab06beaa6ec232e0b83dadaf7e38e53bf43ce48c5`  
		Last Modified: Wed, 24 Feb 2021 19:58:21 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992ef8bddf4ce6ac6f4d3690a4376e7a5a1c4803592eb30b998c0d9d7d07c68d`  
		Last Modified: Wed, 24 Feb 2021 19:58:21 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7760c7347401170d8abd5e8c9b416e7fc26394df85be4aedceb0e4ff0d1800ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115423231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32975631ae125ef47facd0abec967e8e67c9fce89b34e665923f087f38ff1d49`
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
# Wed, 17 Feb 2021 21:24:19 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 21:27:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 17 Feb 2021 21:27:24 GMT
ENV GOPATH=/go
# Wed, 17 Feb 2021 21:27:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 21:27:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 17 Feb 2021 21:27:26 GMT
WORKDIR /go
# Wed, 24 Feb 2021 18:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 18:42:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:42:16 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:42:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:42:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:42:20 GMT
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
	-	`sha256:f02ae61df6c20527527306049385b5821a23bfde3a6c3a4f362322f2c6ad352a`  
		Last Modified: Wed, 17 Feb 2021 21:32:19 GMT  
		Size: 104.8 MB (104803330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a36fe45a5ab3b048d41427533f9442e8ced3ea233c2e8a088013300b0a6400f`  
		Last Modified: Wed, 17 Feb 2021 21:32:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a6e7ca527a8edf1532eb53ef521db466d4fd71c87015f32e725da3921cab88`  
		Last Modified: Wed, 24 Feb 2021 18:43:06 GMT  
		Size: 6.5 MB (6470674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbec22bf82ca9cf6144b7dec23edfe0ceb9983d84d6aa738165e41e9c386385`  
		Last Modified: Wed, 24 Feb 2021 18:43:04 GMT  
		Size: 1.3 MB (1264432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5020a6df6ce3daa929a762f0b9533081ea21a75557c2984301634fc075572a5c`  
		Last Modified: Wed, 24 Feb 2021 18:43:04 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:381f61d19345a344dd3104d80c21ac1007fb0a52e0f66cdb01355036850f683f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619543568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0882e158bf5957cc30e2d0b11c1046ca941a39971831439df44222d849597b93`
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
# Wed, 17 Feb 2021 02:15:15 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 02:17:54 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5cc88fa506b3d5c453c54c3ea218fc8dd05d7362ae1de15bb67986b72089ce93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 17 Feb 2021 02:17:56 GMT
WORKDIR C:\gopath
# Wed, 24 Feb 2021 19:21:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Feb 2021 19:21:19 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:21:21 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:21:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:21:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:21:45 GMT
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
	-	`sha256:3aed69f072632fc0f228c744a84f1143712e5c33b0ffb0bf6fe2e97bb77e3e10`  
		Last Modified: Wed, 17 Feb 2021 02:26:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a42fbe875aa8be5f3c62f490044635a20f9e32992d48f8ac5dd0544817b7348`  
		Last Modified: Wed, 17 Feb 2021 02:26:46 GMT  
		Size: 143.7 MB (143704681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aa6be3ec7c888e6dbb92088273105aebbf62c2b5c9dc6b964413a66e0fae92`  
		Last Modified: Wed, 17 Feb 2021 02:26:16 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b0f7eae8add45f412a9654f869a2e4f64639751c70ba83e8cdf4ec1411c8fd`  
		Last Modified: Wed, 24 Feb 2021 19:26:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44b6fad9135c80957b76d4de90492e2ed1a3154ee473d6473fc5740fccdad2`  
		Last Modified: Wed, 24 Feb 2021 19:25:57 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2e88c6b1456b2b8b0aff5bb1b4d23b241681e3019e1941cbd5b9430b189460`  
		Last Modified: Wed, 24 Feb 2021 19:25:58 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5988cadd604434e562dbf60a5275ee79beaaac9f46ee96a55981a161389dac43`  
		Last Modified: Wed, 24 Feb 2021 19:25:58 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e12ad17f947dbe2370b1a621178f1fcfe4b000db1f9a31b2adb44754f96aba`  
		Last Modified: Wed, 24 Feb 2021 19:26:00 GMT  
		Size: 1.7 MB (1731058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11c022acc8de60694659dbad25fd196ca3befd6c27715779d85e6274a8f500a`  
		Last Modified: Wed, 24 Feb 2021 19:25:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:438d6350303c79a5e6b7139f008e76fd5620acd30c1750b979d43982d968ae44
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5996539423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15595aa105ce7ded6768acf49cfe60bc6e50191cc3eab3656a2e52ce3ea609b`
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
# Wed, 17 Feb 2021 02:18:13 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 02:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5cc88fa506b3d5c453c54c3ea218fc8dd05d7362ae1de15bb67986b72089ce93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 17 Feb 2021 02:21:54 GMT
WORKDIR C:\gopath
# Wed, 24 Feb 2021 19:21:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Feb 2021 19:21:52 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:21:53 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:21:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:23:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:23:10 GMT
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
	-	`sha256:5c10ef0587704099f2dab4cc45e971878e46266b6afd1ddaf7cad6c3b70bd5e4`  
		Last Modified: Wed, 17 Feb 2021 02:27:07 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bfe73165b650064aa4bd52825a640fa1f37fb04c1ab9f868050d11e4671aca`  
		Last Modified: Wed, 17 Feb 2021 02:29:55 GMT  
		Size: 149.1 MB (149115153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbca2b3e0072d60a3ed65c4d69890aa3d6e017e7e29ec50c8187357298cc273d`  
		Last Modified: Wed, 17 Feb 2021 02:27:07 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7bb18c9cf0515093cd58a0d6ad4fd4202628ed9c1af080e34620bcf2253ab8`  
		Last Modified: Wed, 24 Feb 2021 19:26:13 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed0e90a24a1331fddac42be19c09b637beaf666c6cca9c067ab21c1e7e477c`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e8c12462102761054887e694874f02a3bf50e14374452425eb2c852f2f4a08`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e49badf073eea2cf75effcdd44fb32f9c7845321fe5aa91cd38f9ed6e17c523`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00343e2e012dd5f4ea54cf2684f497ce00fdf4125c3cd2dc839ff8355c07449`  
		Last Modified: Wed, 24 Feb 2021 19:26:25 GMT  
		Size: 11.5 MB (11507822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec14d4b1cbfe6b926791a12dcfc5d6a03fe1a673f49d6307a5bae6c53d711d38`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder-alpine`

```console
$ docker pull caddy@sha256:423b6ef6fef24ca01ca00fc111d36531702d51921d209de800b952156d13b9b8
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
$ docker pull caddy@sha256:fb66c744a934e5394fc5f784a2a01e392ee1d4ac871bb7aa73bc53ec44366c46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116485823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ea040656d90666d3f0d3a24d7dffc6c76b95687ca0ec68cd818e56892bc01`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:40:50 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 17 Feb 2021 22:40:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 17 Feb 2021 22:40:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 22:40:51 GMT
ENV GOLANG_VERSION=1.16
# Thu, 25 Feb 2021 04:39:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:39:59 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:39:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:40:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:40:00 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:24 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 25 Feb 2021 05:10:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a078c6c131006663e0108b8cef6955129ece35a6e80457b136ed6aa89e4e11`  
		Last Modified: Wed, 17 Feb 2021 22:51:07 GMT  
		Size: 281.2 KB (281187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f90fd1d94bfeb4d4ed803aed56e7043d6b70c53b2c4abbe8d991d976806ee`  
		Last Modified: Wed, 17 Feb 2021 22:51:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdc4f024afdfc3df10c01e560b5a806ee703b0adf125d232e89ffb4e93dc271`  
		Last Modified: Thu, 25 Feb 2021 04:49:11 GMT  
		Size: 105.7 MB (105693504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b7f786c0727dff7e48f0dd73ffc2e720aa86ce3a3375f2408583d85cd4755a`  
		Last Modified: Thu, 25 Feb 2021 04:48:53 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6ef60a9cbf7b15e2e66c1fe96c2df5ff21ef1e67c2c1b71e87d6937ecefa02`  
		Last Modified: Thu, 25 Feb 2021 05:10:54 GMT  
		Size: 6.4 MB (6387716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9117268777094dec4f2c007e2668dc08fd44f1d444398461654565644e6001`  
		Last Modified: Thu, 25 Feb 2021 05:10:52 GMT  
		Size: 1.3 MB (1311072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8328762831932af440a9a3bb8c34afdef0804dab09132cfbb7973b876d57ad44`  
		Last Modified: Thu, 25 Feb 2021 05:10:52 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:d2b866a0ae711fa875f348fb6417a974ead445204fd5c5a3ea01dbb09a3a5da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112253502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581c9e901c158ef3f74130d144d8f07116224cc9a8719a732e7d8772eceffb08`
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
# Wed, 17 Feb 2021 21:13:48 GMT
ENV GOLANG_VERSION=1.16
# Thu, 25 Feb 2021 03:47:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:48:04 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:48:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:48:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:48:07 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:35:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 25 Feb 2021 04:35:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:35:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:35:08 GMT
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
	-	`sha256:bace9343badd2dadb675a52f16f3ca4ccd112da029eee05d5355e75c0ab4c896`  
		Last Modified: Thu, 25 Feb 2021 03:58:25 GMT  
		Size: 101.9 MB (101903218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5a22f9f0218553919c9ed75b438a84f021bfd75f0fdf31e4606bccd643b73`  
		Last Modified: Thu, 25 Feb 2021 03:48:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f47979b8644c84f4fb66ada27db79035ef367f96c327d01cb9715512220a41`  
		Last Modified: Thu, 25 Feb 2021 04:35:52 GMT  
		Size: 6.2 MB (6224571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda9ebdf27fe5887f1d80c5b1ff2e7e50d4b10f34a18a68a77084595581749d`  
		Last Modified: Thu, 25 Feb 2021 04:35:50 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea394686359ebc055063fd14cdc1f2e1811fb623d6e00dc0e2cbd0336d97c08`  
		Last Modified: Thu, 25 Feb 2021 04:35:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ab4e24de38d7d287168310442ff1608d3289cf1f4eedca5d0ac99674e9563fb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111155980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66a07c48b16e7d8f0feb7c043a34e9ca71d0beeba68bcd923599fa97ece655d`
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
# Wed, 17 Feb 2021 21:40:41 GMT
ENV GOLANG_VERSION=1.16
# Thu, 25 Feb 2021 03:34:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:34:15 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:34:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:34:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:34:19 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:57 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:58 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 25 Feb 2021 04:04:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:04:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:04:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:04:07 GMT
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
	-	`sha256:8b89f1d7fa372cb0e714983a27382a72cd9a5e5f73733b308b2a62f5bb1e3496`  
		Last Modified: Thu, 25 Feb 2021 03:44:43 GMT  
		Size: 101.7 MB (101673489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c84ed09a6a9bd0980324017bfa100dd3e954b188ade04e9e18822b82f18bcf`  
		Last Modified: Thu, 25 Feb 2021 03:44:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93bd526776a73b96e82d27d54ff24510e3d867161d56f4c6f9516ff05b4ce0`  
		Last Modified: Thu, 25 Feb 2021 04:04:44 GMT  
		Size: 5.6 MB (5557907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac831342f93da8aeb2bd524789a3e0622343c77a380b859bae56c5b514737c`  
		Last Modified: Thu, 25 Feb 2021 04:04:43 GMT  
		Size: 1.2 MB (1219449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c0836e37206eaa801b6fa33b09a51a6d781a99fed99103b5df42302ba3618a`  
		Last Modified: Thu, 25 Feb 2021 04:04:43 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:06e2fa7ac82894126d4c59e8ebdb1b3cd35192bd5380628827055df543862103
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111686232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:863624a1a77d720a00482a98e959ecee09e1509f2980e85be0adafb3b3afe501`
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
# Wed, 17 Feb 2021 21:28:34 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 21:30:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 17 Feb 2021 21:30:44 GMT
ENV GOPATH=/go
# Wed, 17 Feb 2021 21:30:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 21:30:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 17 Feb 2021 21:30:50 GMT
WORKDIR /go
# Wed, 24 Feb 2021 18:48:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 18:48:34 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:48:35 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:48:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:48:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:48:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:48:41 GMT
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
	-	`sha256:acb1b01f386a26b11a631443b9b147712664e2b7bb6a08c820259bb6d8dceca5`  
		Last Modified: Wed, 17 Feb 2021 21:34:37 GMT  
		Size: 101.0 MB (101017423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81f77ca7a56bd184d62fd0e65d33077ba482a38e0fa2f128668f9cef65ad766`  
		Last Modified: Wed, 17 Feb 2021 21:34:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c163de3737f8bd6236ce025f7f4620f02a9ffbad6c02df77c7ab1683196de22`  
		Last Modified: Wed, 24 Feb 2021 18:49:32 GMT  
		Size: 6.5 MB (6473491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da6df0249182fed0f9e6c06bf3a2d5328743e1af9d4d16ee374cb5594f5be49`  
		Last Modified: Wed, 24 Feb 2021 18:49:28 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39fc6e66c939043b655941a2d5886aa6fb247601ed47205dc157a82f09f1055`  
		Last Modified: Wed, 24 Feb 2021 18:49:28 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7d5aa30a0c0011b1b4432d0b6b49b49991ebb60becf80be59269cefaf1e0336d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110550372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3afc18a2b038a1d7a452c0c571581412432b0adfcfa5176d56fa8c105934fb`
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
# Wed, 17 Feb 2021 22:01:11 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 22:03:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 17 Feb 2021 22:03:52 GMT
ENV GOPATH=/go
# Wed, 17 Feb 2021 22:03:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 22:04:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 17 Feb 2021 22:04:32 GMT
WORKDIR /go
# Wed, 24 Feb 2021 19:56:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 19:56:39 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:56:42 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:56:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:57:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 19:57:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 19:57:22 GMT
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
	-	`sha256:9111591a7eef4253aba30dd3eae45995c334bf7d627ce834dbf79f283fa1bb48`  
		Last Modified: Wed, 17 Feb 2021 22:08:49 GMT  
		Size: 99.5 MB (99460179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d30531ced472075060419d974e043566600f535317ecb701b4183ca3ce76936`  
		Last Modified: Wed, 17 Feb 2021 22:08:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ec9433e8ec8bc30b8d6c1ef4e505c341111ef0430e62a2771ad178d28c19f0`  
		Last Modified: Wed, 24 Feb 2021 19:58:23 GMT  
		Size: 6.8 MB (6822502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0159ae43773b5a368197692ab06beaa6ec232e0b83dadaf7e38e53bf43ce48c5`  
		Last Modified: Wed, 24 Feb 2021 19:58:21 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992ef8bddf4ce6ac6f4d3690a4376e7a5a1c4803592eb30b998c0d9d7d07c68d`  
		Last Modified: Wed, 24 Feb 2021 19:58:21 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7760c7347401170d8abd5e8c9b416e7fc26394df85be4aedceb0e4ff0d1800ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115423231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32975631ae125ef47facd0abec967e8e67c9fce89b34e665923f087f38ff1d49`
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
# Wed, 17 Feb 2021 21:24:19 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 21:27:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.src.tar.gz'; 	sha256='7688063d55656105898f323d90a79a39c378d86fe89ae192eb3b7fc46347c95a'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 17 Feb 2021 21:27:24 GMT
ENV GOPATH=/go
# Wed, 17 Feb 2021 21:27:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 21:27:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 17 Feb 2021 21:27:26 GMT
WORKDIR /go
# Wed, 24 Feb 2021 18:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 18:42:16 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:42:16 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 18:42:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:42:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:42:20 GMT
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
	-	`sha256:f02ae61df6c20527527306049385b5821a23bfde3a6c3a4f362322f2c6ad352a`  
		Last Modified: Wed, 17 Feb 2021 21:32:19 GMT  
		Size: 104.8 MB (104803330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a36fe45a5ab3b048d41427533f9442e8ced3ea233c2e8a088013300b0a6400f`  
		Last Modified: Wed, 17 Feb 2021 21:32:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a6e7ca527a8edf1532eb53ef521db466d4fd71c87015f32e725da3921cab88`  
		Last Modified: Wed, 24 Feb 2021 18:43:06 GMT  
		Size: 6.5 MB (6470674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbec22bf82ca9cf6144b7dec23edfe0ceb9983d84d6aa738165e41e9c386385`  
		Last Modified: Wed, 24 Feb 2021 18:43:04 GMT  
		Size: 1.3 MB (1264432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5020a6df6ce3daa929a762f0b9533081ea21a75557c2984301634fc075572a5c`  
		Last Modified: Wed, 24 Feb 2021 18:43:04 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4c96dee7dde83c857d6bb357f4fe148d3e015b49b18bcac42804f447bbf7ab9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.4.0-beta.1-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:381f61d19345a344dd3104d80c21ac1007fb0a52e0f66cdb01355036850f683f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619543568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0882e158bf5957cc30e2d0b11c1046ca941a39971831439df44222d849597b93`
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
# Wed, 17 Feb 2021 02:15:15 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 02:17:54 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5cc88fa506b3d5c453c54c3ea218fc8dd05d7362ae1de15bb67986b72089ce93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 17 Feb 2021 02:17:56 GMT
WORKDIR C:\gopath
# Wed, 24 Feb 2021 19:21:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Feb 2021 19:21:19 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:21:21 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:21:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:21:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:21:45 GMT
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
	-	`sha256:3aed69f072632fc0f228c744a84f1143712e5c33b0ffb0bf6fe2e97bb77e3e10`  
		Last Modified: Wed, 17 Feb 2021 02:26:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a42fbe875aa8be5f3c62f490044635a20f9e32992d48f8ac5dd0544817b7348`  
		Last Modified: Wed, 17 Feb 2021 02:26:46 GMT  
		Size: 143.7 MB (143704681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aa6be3ec7c888e6dbb92088273105aebbf62c2b5c9dc6b964413a66e0fae92`  
		Last Modified: Wed, 17 Feb 2021 02:26:16 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b0f7eae8add45f412a9654f869a2e4f64639751c70ba83e8cdf4ec1411c8fd`  
		Last Modified: Wed, 24 Feb 2021 19:26:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44b6fad9135c80957b76d4de90492e2ed1a3154ee473d6473fc5740fccdad2`  
		Last Modified: Wed, 24 Feb 2021 19:25:57 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2e88c6b1456b2b8b0aff5bb1b4d23b241681e3019e1941cbd5b9430b189460`  
		Last Modified: Wed, 24 Feb 2021 19:25:58 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5988cadd604434e562dbf60a5275ee79beaaac9f46ee96a55981a161389dac43`  
		Last Modified: Wed, 24 Feb 2021 19:25:58 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e12ad17f947dbe2370b1a621178f1fcfe4b000db1f9a31b2adb44754f96aba`  
		Last Modified: Wed, 24 Feb 2021 19:26:00 GMT  
		Size: 1.7 MB (1731058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11c022acc8de60694659dbad25fd196ca3befd6c27715779d85e6274a8f500a`  
		Last Modified: Wed, 24 Feb 2021 19:25:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9046bac3cf0034d2f570829d45fc353f3eee53dfe83a9080230aea79d329d973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.4.0-beta.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:438d6350303c79a5e6b7139f008e76fd5620acd30c1750b979d43982d968ae44
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5996539423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15595aa105ce7ded6768acf49cfe60bc6e50191cc3eab3656a2e52ce3ea609b`
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
# Wed, 17 Feb 2021 02:18:13 GMT
ENV GOLANG_VERSION=1.16
# Wed, 17 Feb 2021 02:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5cc88fa506b3d5c453c54c3ea218fc8dd05d7362ae1de15bb67986b72089ce93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 17 Feb 2021 02:21:54 GMT
WORKDIR C:\gopath
# Wed, 24 Feb 2021 19:21:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Feb 2021 19:21:52 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:21:53 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:21:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:23:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:23:10 GMT
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
	-	`sha256:5c10ef0587704099f2dab4cc45e971878e46266b6afd1ddaf7cad6c3b70bd5e4`  
		Last Modified: Wed, 17 Feb 2021 02:27:07 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bfe73165b650064aa4bd52825a640fa1f37fb04c1ab9f868050d11e4671aca`  
		Last Modified: Wed, 17 Feb 2021 02:29:55 GMT  
		Size: 149.1 MB (149115153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbca2b3e0072d60a3ed65c4d69890aa3d6e017e7e29ec50c8187357298cc273d`  
		Last Modified: Wed, 17 Feb 2021 02:27:07 GMT  
		Size: 1.6 KB (1586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7bb18c9cf0515093cd58a0d6ad4fd4202628ed9c1af080e34620bcf2253ab8`  
		Last Modified: Wed, 24 Feb 2021 19:26:13 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed0e90a24a1331fddac42be19c09b637beaf666c6cca9c067ab21c1e7e477c`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e8c12462102761054887e694874f02a3bf50e14374452425eb2c852f2f4a08`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e49badf073eea2cf75effcdd44fb32f9c7845321fe5aa91cd38f9ed6e17c523`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00343e2e012dd5f4ea54cf2684f497ce00fdf4125c3cd2dc839ff8355c07449`  
		Last Modified: Wed, 24 Feb 2021 19:26:25 GMT  
		Size: 11.5 MB (11507822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec14d4b1cbfe6b926791a12dcfc5d6a03fe1a673f49d6307a5bae6c53d711d38`  
		Last Modified: Wed, 24 Feb 2021 19:26:09 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-windowsservercore`

```console
$ docker pull caddy@sha256:daa27c3e4db7f292cef9a4f15d2d6ee28f3f984f5f9d6f32137ac79ee1a6ed64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.4.0-beta.1-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4cdeba0900efe52172abfbcaba09cbf73eb331dd494069ce5d7d3edf60aef105
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465520956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4da660c15226e24c8818c56bcd37329210b1be2f7f7a7685824dd821cf87e4`
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
# Wed, 24 Feb 2021 19:17:36 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:18:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 24 Feb 2021 19:18:07 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 24 Feb 2021 19:18:09 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 24 Feb 2021 19:18:10 GMT
VOLUME [c:/config]
# Wed, 24 Feb 2021 19:18:11 GMT
VOLUME [c:/data]
# Wed, 24 Feb 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:18:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:18:21 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:18:22 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:18:23 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:18:38 GMT
RUN caddy version
# Wed, 24 Feb 2021 19:18:39 GMT
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
	-	`sha256:f329d3bba024566dab2f54071c6fba793f7fc404fc263b3aabb7601c9bf2fb2f`  
		Last Modified: Wed, 24 Feb 2021 19:25:02 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0eee823ef67f2c681b991fe34c0d27d2a44fa8bf09aa82dd505ba02b96cead`  
		Last Modified: Wed, 24 Feb 2021 19:25:06 GMT  
		Size: 16.5 MB (16493289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2210192c57f0a5c9bcbe3ab21f13741fd237b6420b8c670eed14a22a16ee80bb`  
		Last Modified: Wed, 24 Feb 2021 19:24:59 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d3f637f6812bd743380eebe8562e9eceaf5c6f8fccb74dcdfa8c5c155676e`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6704bc8ecdf53603807915f467f051697beb2db554852b9e20ea0ba6e79a2`  
		Last Modified: Wed, 24 Feb 2021 19:24:57 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ba0394b89181a0a2a9f8f4c14cbe4071c17bade6f66e0932dca617c8504bd`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c5104a4e7bc41571751f57783252f586c119a2e53e95224b18b98df981991`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927608485d189dbdd46f2b6a3143e94cb5546ea4d8baaeb31008d8217ab1d10`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d07473d7282ce10d7338969fa4a521267f81eaefaf34bebb643ca2f36c506`  
		Last Modified: Wed, 24 Feb 2021 19:24:53 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886d84a62de83fb3db42795e623d933b7c6d7c060310dfd26a999216c198020`  
		Last Modified: Wed, 24 Feb 2021 19:24:51 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a0c8d74f92a4f3a0cf6010e0a694402535f0e7c9aa7f3c23a43b5658180927`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cbae6a4753f68cc678ccff331d7979824475f16e5347a7f642bb0623366d3`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0076f0ebea58934879757debf312e4720988c27c090a78f2cf86585dc0f2b0`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7a116da5f39e6bb191c00a41dcab7309e8fa3c5c75a1c8cd4a298923db823e`  
		Last Modified: Wed, 24 Feb 2021 19:24:51 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a35eec38e96847beea1ab1041a962421f9da53734c8d2aeda03fe21451ab385`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5ade964bcedfaa3d1305c7630f31fc759157cc72491a8b3b3927bab60e977`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c81a658875f96063212596f9c09e82dd68db7e0bb52595402ae4ada2865ad9`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0b796ca125b226c1c29c71496c5a1909375b96c2ca437586ff519ede12434`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 310.0 KB (310045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefe957f99ec30bdadabfe9d1e567a62f6b9ea7e0a2a823606e07f16466d42c`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:ddaa5a644e0bf998397932e079929ef88eefd667e91007b58db748808ea3753b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827363881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bb9bdf3d216ef29abbd04a4936b94a7287286b88c3d15d550d8a07880e826e`
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
# Wed, 24 Feb 2021 19:18:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:20:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 24 Feb 2021 19:20:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 24 Feb 2021 19:20:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 24 Feb 2021 19:20:13 GMT
VOLUME [c:/config]
# Wed, 24 Feb 2021 19:20:14 GMT
VOLUME [c:/data]
# Wed, 24 Feb 2021 19:20:15 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:20:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:20:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:20:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:20:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:20:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:20:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:20:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:20:24 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:20:25 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:20:26 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:21:07 GMT
RUN caddy version
# Wed, 24 Feb 2021 19:21:08 GMT
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
	-	`sha256:620b960cc16ddec3206afd68382c040b072539c2cf01242c1e4b5a5dfca7d028`  
		Last Modified: Wed, 24 Feb 2021 19:25:27 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a31f0da573a4abd5d0843b1660aa4f5e2ab59b1ec4d8ccf225b1f3d35c597c`  
		Last Modified: Wed, 24 Feb 2021 19:25:48 GMT  
		Size: 21.9 MB (21886898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb06c4c8131855b07a7e6aedf897493c47175ba4dc276d26cfebd4b4098595fb`  
		Last Modified: Wed, 24 Feb 2021 19:25:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dc50f20b45c1477c56f840dc00ef32901efae31ed270d7dd8e8845ca64720b`  
		Last Modified: Wed, 24 Feb 2021 19:25:26 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6703e6122eb70ecd05222f36b06445d6e2c2aefdc019fb5b0341241e652a53`  
		Last Modified: Wed, 24 Feb 2021 19:25:22 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf3790132d185f7e33b7053b6f4dda7c7e28a06b4f1d32854f67a3cd04dccb0`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47157fb5a89d548d92f0b15ec5ec80a9d17c893aea9803ca5a0c0f9219fc6ec0`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e55b1c202dbdf0fe8326434a42ff3595e08e3f9cfde195aa51392db7f28f8`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33ee4c38831d27e736ad2e1c0594afee3d66c737928c5a1d7559845b4e1c28b`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9dd6b6a2798e8046294e2f0f344a10ae3abbde16affc3503250a7a831c5534`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6210a68b0d3529c79c68790765bb978c0670600837a00a1459b9224e0c163bcc`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afdaf4879538ca073c8a1713e8da86b01c686d3a2c0eecf13dab42d42334416`  
		Last Modified: Wed, 24 Feb 2021 19:25:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf56b89756efdcac0787d0e591907289fbbe3b9a52a0a0f23e522407dd06be`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a758a2e5470fa296d7d2502ab3d42444ce8952a1a81d9afcaadb8413355b89`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935097fef5cb53c8029a6d7c1bb86f992eee3b23c3299f1a8c8b7ce4431bef34`  
		Last Modified: Wed, 24 Feb 2021 19:25:15 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271677474997ecda9d71f27b0e98a3e37177ffa4300e7722f43cb4d159105f61`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5843ab6da12a2b587a4cc80bcc23f45340c43cd6b1f654f25b59d9d7ebd4fb7`  
		Last Modified: Wed, 24 Feb 2021 19:25:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d053551a5b55945e305bf63d8ab4bf9b0c6d009c83b05b1e3566f6b2bf04d`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 260.6 KB (260550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970166f3bfb7d87cfcf06548a018973d37f49049b2f451706eecb6d03a98c349`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:b2f9133e29253b076ab35988f9a84903c200d95402906982f4b73216a8192751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2.4.0-beta.1-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4cdeba0900efe52172abfbcaba09cbf73eb331dd494069ce5d7d3edf60aef105
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465520956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4da660c15226e24c8818c56bcd37329210b1be2f7f7a7685824dd821cf87e4`
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
# Wed, 24 Feb 2021 19:17:36 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:18:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 24 Feb 2021 19:18:07 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 24 Feb 2021 19:18:09 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 24 Feb 2021 19:18:10 GMT
VOLUME [c:/config]
# Wed, 24 Feb 2021 19:18:11 GMT
VOLUME [c:/data]
# Wed, 24 Feb 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:18:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:18:21 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:18:22 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:18:23 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:18:38 GMT
RUN caddy version
# Wed, 24 Feb 2021 19:18:39 GMT
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
	-	`sha256:f329d3bba024566dab2f54071c6fba793f7fc404fc263b3aabb7601c9bf2fb2f`  
		Last Modified: Wed, 24 Feb 2021 19:25:02 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0eee823ef67f2c681b991fe34c0d27d2a44fa8bf09aa82dd505ba02b96cead`  
		Last Modified: Wed, 24 Feb 2021 19:25:06 GMT  
		Size: 16.5 MB (16493289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2210192c57f0a5c9bcbe3ab21f13741fd237b6420b8c670eed14a22a16ee80bb`  
		Last Modified: Wed, 24 Feb 2021 19:24:59 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d3f637f6812bd743380eebe8562e9eceaf5c6f8fccb74dcdfa8c5c155676e`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6704bc8ecdf53603807915f467f051697beb2db554852b9e20ea0ba6e79a2`  
		Last Modified: Wed, 24 Feb 2021 19:24:57 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ba0394b89181a0a2a9f8f4c14cbe4071c17bade6f66e0932dca617c8504bd`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c5104a4e7bc41571751f57783252f586c119a2e53e95224b18b98df981991`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927608485d189dbdd46f2b6a3143e94cb5546ea4d8baaeb31008d8217ab1d10`  
		Last Modified: Wed, 24 Feb 2021 19:24:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630d07473d7282ce10d7338969fa4a521267f81eaefaf34bebb643ca2f36c506`  
		Last Modified: Wed, 24 Feb 2021 19:24:53 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886d84a62de83fb3db42795e623d933b7c6d7c060310dfd26a999216c198020`  
		Last Modified: Wed, 24 Feb 2021 19:24:51 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a0c8d74f92a4f3a0cf6010e0a694402535f0e7c9aa7f3c23a43b5658180927`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cbae6a4753f68cc678ccff331d7979824475f16e5347a7f642bb0623366d3`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0076f0ebea58934879757debf312e4720988c27c090a78f2cf86585dc0f2b0`  
		Last Modified: Wed, 24 Feb 2021 19:24:50 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7a116da5f39e6bb191c00a41dcab7309e8fa3c5c75a1c8cd4a298923db823e`  
		Last Modified: Wed, 24 Feb 2021 19:24:51 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a35eec38e96847beea1ab1041a962421f9da53734c8d2aeda03fe21451ab385`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5ade964bcedfaa3d1305c7630f31fc759157cc72491a8b3b3927bab60e977`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c81a658875f96063212596f9c09e82dd68db7e0bb52595402ae4ada2865ad9`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0b796ca125b226c1c29c71496c5a1909375b96c2ca437586ff519ede12434`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 310.0 KB (310045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefe957f99ec30bdadabfe9d1e567a62f6b9ea7e0a2a823606e07f16466d42c`  
		Last Modified: Wed, 24 Feb 2021 19:24:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:7b437513ca5285ea1315abb00a5c9f46ad8e50fb99d0c1b1986f963947b23316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2.4.0-beta.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:ddaa5a644e0bf998397932e079929ef88eefd667e91007b58db748808ea3753b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827363881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bb9bdf3d216ef29abbd04a4936b94a7287286b88c3d15d550d8a07880e826e`
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
# Wed, 24 Feb 2021 19:18:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:20:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5f04847c2bdd4526fb690c95710a6a0583e213182024b4844f3ea2fdabf78593474bfcfbd1f96e53d464eb9c925b8c040c7dc92968ac9dba547861e88fce8fd5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 24 Feb 2021 19:20:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 24 Feb 2021 19:20:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 24 Feb 2021 19:20:13 GMT
VOLUME [c:/config]
# Wed, 24 Feb 2021 19:20:14 GMT
VOLUME [c:/data]
# Wed, 24 Feb 2021 19:20:15 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 24 Feb 2021 19:20:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 19:20:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 19:20:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 19:20:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 19:20:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 19:20:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 19:20:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 19:20:24 GMT
EXPOSE 80
# Wed, 24 Feb 2021 19:20:25 GMT
EXPOSE 443
# Wed, 24 Feb 2021 19:20:26 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 19:21:07 GMT
RUN caddy version
# Wed, 24 Feb 2021 19:21:08 GMT
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
	-	`sha256:620b960cc16ddec3206afd68382c040b072539c2cf01242c1e4b5a5dfca7d028`  
		Last Modified: Wed, 24 Feb 2021 19:25:27 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a31f0da573a4abd5d0843b1660aa4f5e2ab59b1ec4d8ccf225b1f3d35c597c`  
		Last Modified: Wed, 24 Feb 2021 19:25:48 GMT  
		Size: 21.9 MB (21886898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb06c4c8131855b07a7e6aedf897493c47175ba4dc276d26cfebd4b4098595fb`  
		Last Modified: Wed, 24 Feb 2021 19:25:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dc50f20b45c1477c56f840dc00ef32901efae31ed270d7dd8e8845ca64720b`  
		Last Modified: Wed, 24 Feb 2021 19:25:26 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6703e6122eb70ecd05222f36b06445d6e2c2aefdc019fb5b0341241e652a53`  
		Last Modified: Wed, 24 Feb 2021 19:25:22 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf3790132d185f7e33b7053b6f4dda7c7e28a06b4f1d32854f67a3cd04dccb0`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47157fb5a89d548d92f0b15ec5ec80a9d17c893aea9803ca5a0c0f9219fc6ec0`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e55b1c202dbdf0fe8326434a42ff3595e08e3f9cfde195aa51392db7f28f8`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33ee4c38831d27e736ad2e1c0594afee3d66c737928c5a1d7559845b4e1c28b`  
		Last Modified: Wed, 24 Feb 2021 19:25:21 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9dd6b6a2798e8046294e2f0f344a10ae3abbde16affc3503250a7a831c5534`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6210a68b0d3529c79c68790765bb978c0670600837a00a1459b9224e0c163bcc`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afdaf4879538ca073c8a1713e8da86b01c686d3a2c0eecf13dab42d42334416`  
		Last Modified: Wed, 24 Feb 2021 19:25:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf56b89756efdcac0787d0e591907289fbbe3b9a52a0a0f23e522407dd06be`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a758a2e5470fa296d7d2502ab3d42444ce8952a1a81d9afcaadb8413355b89`  
		Last Modified: Wed, 24 Feb 2021 19:25:18 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935097fef5cb53c8029a6d7c1bb86f992eee3b23c3299f1a8c8b7ce4431bef34`  
		Last Modified: Wed, 24 Feb 2021 19:25:15 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271677474997ecda9d71f27b0e98a3e37177ffa4300e7722f43cb4d159105f61`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5843ab6da12a2b587a4cc80bcc23f45340c43cd6b1f654f25b59d9d7ebd4fb7`  
		Last Modified: Wed, 24 Feb 2021 19:25:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d053551a5b55945e305bf63d8ab4bf9b0c6d009c83b05b1e3566f6b2bf04d`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 260.6 KB (260550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970166f3bfb7d87cfcf06548a018973d37f49049b2f451706eecb6d03a98c349`  
		Last Modified: Wed, 24 Feb 2021 19:25:16 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:186302fda6b402513edbfe8ff920e13d096d2838b43757ea2718a36ef79a54b8
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
$ docker pull caddy@sha256:9c7988221ae79035b2451e3747a0ecdd8431be642132626a2d113493d0340f9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2160ea65c1af29529ed745aa66e384c6bf69b6476cb887c7f5c20be899abd260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:01:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:01:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:01:29 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:01:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:01:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:01:35 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:01:36 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:01:38 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:01:39 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:01:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e943fcd90b84a982b5885d766383fe0854ebe777f92c4e607d3ac1410cf06e`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 299.9 KB (299950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bb94c554bfa30e776d58e02f639b022f13f4f8d28f2ea51fe1569d0f3342b`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ec0fb337e64a01607417a0d90cbfa0cf4937a4609bce91892ce3c518332d2`  
		Last Modified: Wed, 24 Feb 2021 21:02:26 GMT  
		Size: 11.6 MB (11622361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0e4e5582798cbcbf63965ea2dac6d5e93471bb0f62074d572c2d9806fcc8`  
		Last Modified: Wed, 24 Feb 2021 21:02:23 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:639e197fa1970e89c9466452a95e9701fc3d06ad5f85d4c4cf7fcf51875de656
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
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
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
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
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
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
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
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
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
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
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
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
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
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
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
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
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
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
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
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
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
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
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
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
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
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
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
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
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
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:6847eff581ebbf642621d409c59845c6991e154136045f3ed113b337366bc5d0
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
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
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
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
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
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
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
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
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
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
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
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
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
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
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
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
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
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
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
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
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
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb33c8de1233228709c51b4f60dc46b9c661051664b72b9677728f592fb795c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
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
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
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
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:8e5dcc2f90feef29505c8c129dd01f248bfd711239067688d5e3f62344e0e98a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
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
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
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
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
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
$ docker pull caddy@sha256:186302fda6b402513edbfe8ff920e13d096d2838b43757ea2718a36ef79a54b8
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
$ docker pull caddy@sha256:9c7988221ae79035b2451e3747a0ecdd8431be642132626a2d113493d0340f9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2160ea65c1af29529ed745aa66e384c6bf69b6476cb887c7f5c20be899abd260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:01:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:01:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:01:29 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:01:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:01:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:01:35 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:01:36 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:01:38 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:01:39 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:01:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e943fcd90b84a982b5885d766383fe0854ebe777f92c4e607d3ac1410cf06e`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 299.9 KB (299950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bb94c554bfa30e776d58e02f639b022f13f4f8d28f2ea51fe1569d0f3342b`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ec0fb337e64a01607417a0d90cbfa0cf4937a4609bce91892ce3c518332d2`  
		Last Modified: Wed, 24 Feb 2021 21:02:26 GMT  
		Size: 11.6 MB (11622361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0e4e5582798cbcbf63965ea2dac6d5e93471bb0f62074d572c2d9806fcc8`  
		Last Modified: Wed, 24 Feb 2021 21:02:23 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:639e197fa1970e89c9466452a95e9701fc3d06ad5f85d4c4cf7fcf51875de656
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
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
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
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
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
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
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
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
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
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
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
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
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
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
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
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
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
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
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
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
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
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
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
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
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
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
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
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
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
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:6847eff581ebbf642621d409c59845c6991e154136045f3ed113b337366bc5d0
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
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
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
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
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
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
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
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
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
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
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
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
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
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
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
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
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
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
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
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
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
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fb33c8de1233228709c51b4f60dc46b9c661051664b72b9677728f592fb795c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
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
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
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
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:8e5dcc2f90feef29505c8c129dd01f248bfd711239067688d5e3f62344e0e98a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
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
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
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
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:72da1ab397f9f002ad371ff4ae4c4b477a9c9fe73f37e87de981ae4c98986280
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
$ docker pull caddy@sha256:9c7988221ae79035b2451e3747a0ecdd8431be642132626a2d113493d0340f9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14727708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2160ea65c1af29529ed745aa66e384c6bf69b6476cb887c7f5c20be899abd260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:01:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:01:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:01:29 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:01:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:01:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:01:35 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:01:35 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:01:36 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:01:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:01:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:01:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:01:38 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:01:39 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:01:39 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:01:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e943fcd90b84a982b5885d766383fe0854ebe777f92c4e607d3ac1410cf06e`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 299.9 KB (299950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bb94c554bfa30e776d58e02f639b022f13f4f8d28f2ea51fe1569d0f3342b`  
		Last Modified: Wed, 24 Feb 2021 21:02:22 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ec0fb337e64a01607417a0d90cbfa0cf4937a4609bce91892ce3c518332d2`  
		Last Modified: Wed, 24 Feb 2021 21:02:26 GMT  
		Size: 11.6 MB (11622361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0e4e5582798cbcbf63965ea2dac6d5e93471bb0f62074d572c2d9806fcc8`  
		Last Modified: Wed, 24 Feb 2021 21:02:23 GMT  
		Size: 154.0 B  
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
